# Snark_Robot_SLAM_V2
IQ Robot base systems using L02 SLAM Nav System

The RV1001AED series robot utilizes an uppward facing camera for visual tracking paired with odometry data.

The SOC for the navigation system is the Rockchip RK3326 quad core 1.3Ghz with 512Mb (2x 256Mb) DDR, and 4Gb of emmc storage.

Using the ADC_Key input, I found that a 20mV input or less will cause the L02 to boot in to a recovery mode. 
This recovery mode is a basic ramfs utilizing busybox with minimally mounted partitions. I did find I could mount the OEM and rootfs partitions.
With the rootfs partition being squashfs I could not easy modifiy anything since it is mounted read-only. Kermit is not avaliable, and in this mode the WiFi interface is not avaliable. Manually copying and pasting that much data through the serial console does not sound like fun.
In an attempt to get any sort of external storage to work,I made the system go borken!

off to ebay, and $24 later, I have another on the way.


------------------------------More to come soon-------------------------------------------------------------------------------------------
