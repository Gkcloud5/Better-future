#### Source:
[TP](https://www.tutorialspoint.com/unix/unix-pipes-filters.htm)

* we can connect two commands together so that the output from one program becomes the input of the next program.
* `|`, this is pipe

#### Grep command:

```
grep pattern file(s)
```

* g/re/p --> Globally search for a regular expression and print all lines containing it.

```
ls -l | grep "Aug"
```

* -v ==> print all lines that do not match pattern
* -n ==> print matched line and line number

![[Pasted image 20230601075804.png]]


#### sort command:

* this command used to arranges lines of text alphabetically or numerically.

```
sort filename
```

![[Pasted image 20230601075922.png]]

