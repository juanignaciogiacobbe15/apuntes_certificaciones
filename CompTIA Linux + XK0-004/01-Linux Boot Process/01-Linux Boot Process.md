# Linux Boot Process
1. After a computer starts, the BIOS on the motherboard checks on all of the hardware and IO devices. -> Everything checks out, and the boot process for the computer can begin.
2. The boot program will look for the section of the hard drive that contains the data needed to boot an OS -> The bootloader will then load the Linux Kernel.
3. The Kernel will then load what is called an initial RAM disk, which contains a bunch of device drivers and starts to load the computer's drivers to eventually mount the File System from the hard disk.
4. After the Kernel is all set up and ready to go, it then starts off the initialization system.

![](../img/Pasted%20image%2020240923123231.png)

5. Once the Initialization System starts, it takes over mounting the computer's File Systems. At this point, the initial RAM disk is no longer needed and gets removed.
6. The Initialization System continues to load services, and gets the computer in a state where it can be used.

## Boot logs

- The traditional utility used for viewing the kernel ring buffer.
```
dmesg
```

- To view the Kernel ring buffer within the systemd journal.
```
jounalctl -k
```