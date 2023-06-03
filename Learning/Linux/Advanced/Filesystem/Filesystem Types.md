#### Source:
[LJ](https://linuxjourney.com/lesson/filesystem-types)


* There are many different filesystem implementations available.
	* Some are faster than others
	* Some supports larger capacity storage
* Different filesystems have different ways of organizing their data.


#### Journaling:

* Journaling comes by default on most filesystem types.
* Let's say you're copying a large file and all of a sudden you lose power. well if you are on a non-journaled filesystem, the file would end up corrupted and your filesystem would be inconsistent and then when you boot back up,
	* Your system would perform a filesystem check to make everything okay.
	* However, the repair could take awhile depending on how large your filesystem was.
* Now if you were on a journaled system, before your machine even begins to copy the file, it will write what you are going to be doing in a log file(journal). now when you actually copy the file, once it completes, the journal marks that task as complete.
	* The filesystem is always in a consistent state because of this, so it will know exactly where you left off it your machine shutdown suddenly, this also decrease the boot time because instead of checking the entire filesystem it just looks at your journal.


#### Common Desktop filesystem types:

* **ext4:** 
	* This is most current version of the native filesystems.
* **Btrfs:**
	* Better or Butter FS
	* It is new filesystem for linux that comes with snapshots, incremental backups, performance increase and much more.
* **XFS:**
	* High performance journaling file system, great for a system with large files such as media server.
* **NTFS and FAT:**
	* Windows filesystems
* **HFS+:**
	* Macintosh filesystem

```
df -T
```

![[Pasted image 20230602230440.png]]
