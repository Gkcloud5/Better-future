#### Source:
[LJ](https://linuxjourney.com/lesson/filesystem-repair)

* Sometimes our filesystem is not always in the best condition.
* If we have sudden shutdown, our data can become corrupt, it's up to the system to try to get us back in a working state.
* `fsck` command is used to check the consistency of a filesystem and even you can repair it.
* When booting fsck is check disk status before it mounting.

```
fsck /dev/diskname
```

[MAN](https://linux.die.net/man/8/fsck)
