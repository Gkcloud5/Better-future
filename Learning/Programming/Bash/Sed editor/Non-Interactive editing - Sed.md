---
creation date: 2023-06-20 17:54
modification date: Tuesday 20th June 2023 17:54:38
---

**Tags:** #linux #bash #sed

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_05_03.html)

--------------------------------------

#### Explanation about it:

##### Reading sed commands from a file

* Multiple `sed` commands can be put in a file and executed using the `-f` option.
	* No trailing white spaces exist at the end of lines
	* No quotes are used
	* When entering text to add or replace, all except the last line end in a backslash


##### Writing output files:

```
cat script.sed

1i\
<html>\
<head><title>sed generated html</title></head>\
<body bgcolor="#ffffff">\
<pre>
$a\
</pre>\
</body>\
</html>
```


```
cat txt2html.sh

#!/bin/bash

# This is a simple script that you can use for converting text into HTML.
# First we take out all newline characters, so that the appending only happens
# once, then we replace the newlines.

echo "converting $1..."

SCRIPT="/root/bash_script/sed_example/script.sed"
NAME="$1"
TEMPFILE="/var/tmp/sed.$PID.tmp"
sed "s/\n/^M/" $1 | sed -f $SCRIPT | sed "s/^M/\n/" > $TEMPFILE
mv $TEMPFILE $NAME

echo "done."
```


```
cat test

Gk1
Gk2
Gk3
```

#### Output:

```
root@root:~/bash_script/sed_example# cat test
<html>
<head><title>sed generated html</title></head>
<body bgcolor="#ffffff">
<pre>
Gk1
Gk2
Gk3
</pre>
</body>
</html>

```



![[Pasted image 20230621163100.png]]


