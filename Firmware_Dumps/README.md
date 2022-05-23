Any firmware I am able to dump will be posted here.

As of right now I can only dump the first 32Mb of information on the emmc.
There seems to be an issue with the loader image using an unsigned short in the length field.
Since each block is 512Kb, 32Mb of blocks would be decimal 65,535 which is also equal to hex 0xFFFF.

What this has had an affect on is the boot partition. This is where the kernel lives.
A very large chunk of the kernel has been recovered, and it was cut off at a large area of NULL bytes.
If this area of NULL bytes continues to the end of the partition, or of it is an island with data further down; I don't know.

What has been recovered is the: uboot partition, trust boot loader, misc partition (all NULL), and a decent chunck of the boot partition.

A good sign is the trust partition is very sparse, and seems like the firmware with compiled with the headers included for trust, but it was not implemented.
