#### Source:
[LJ](https://linuxjourney.com/lesson/swap-space)

* Swap is used to allocate virtual memory to our system. if you are low on memory, the system uses this partition to swap pieces of memory of idle processes to the disk.

#### Procedure to create a swap:

1. First we make sure we don't have anything on the partition
2. `mkswap /dev/diskpart1` to initialize swap areas.
3. `swapon /dev/diskpart1` this will enable the swap device.
4. if you want swap partition to persist on bootup, you need to add an entry to the /etc/fstab file
5. remove `swapoff /dev/diskpart1`

* Generally you should allocate about twice as much swap space as you have memory.