#### Source:
[LJ](https://linuxjourney.com/lesson/filesystem-types)


* There are many different filesystem implementations available.
	* Some are faster than others
	* Some supports larger capacity storage
* Different filesystems have different ways of organizing their data.


#### Journaling:

* Journaling comes by default on most filesystem types.
* Let's say you're copying a large file and all of a sudden you lose power. well if you are on a non-journaled filesystem, the file would end up corrupted and your filesystem would be inconsistent and then when you boot back up,
	* Your system would perform a filesystem check