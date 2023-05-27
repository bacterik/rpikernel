## Raspbery Pi Kernel - Debian

This custom kernel is compile for Debian native images found at **http://raspi.debian.net**.
The kernel included in these images a pretty generic. This kernel will enable your Raspberry Pi system to fully functional as it should be. This **WONT** work for your Raspberyr PiOS, since /boot directories are different from Debian. 

This kernel is also compiled with a PREEM settings of 250hz, which is a good (better) middle ground. Everything else is set a default, no changes.

This Kernel will identify itself under the APT manager as "linux-image-z10" and as 6.1.21-z10 under "uname" for a somewhat unique naming.
