---
creation date: 2023-06-19 13:04
modification date: Monday 19th June 2023 13:04:20
---

**Tags:** #linux #bash 

#### Source:
[Bash](https://tldp.org/LDP/Bash-Beginners-Guide/html/sect_03_05.html)

--------------------------------------

#### Explanation about it:

##### What are aliases?

* An alias allows a string to be substituted for a word when it is used as the first word of a simple command.

```
root@root:~# alias
alias egrep='egrep --color=auto'
alias fgrep='fgrep --color=auto'
alias grep='grep --color=auto'
alias l='ls -CF'
alias la='ls -A'
alias ll='ls -alF'
alias ls='ls --color=auto'

```

```
#create alias
alias dh="df -h"
dh


#remove alias
unalias dh
```

