## Debian RPI - Kernel, libraries & utils.

This "custom" kernel is compiled for Debian native images found at **http://raspi.debian.net**.
The kernel included in these images a pretty generic. This kernel will enable your Raspberry Pi (under Debian) system to fully functional as it should be. This **WONT** work for your Raspberyr PiOS, since /boot directories are different from Debian.

This kernel is also compiled with a PREEM settings of 250hz, which is a good (better) middle ground, and cpu govenor "on demand". Everything else is set a default, no changes. This kernel includes support for all RPI boards v7/v8.

This Kernel will identify itself under the APT manager as "linux-image-z10" and as 6.1.x-z10 under "uname" for a somewhat unique naming.

Install with:

dpkg -i filename.deb

- Dont forget to:

Pruge the Debian default kernel "linux-image-x" and anwser YES to "Remove current running kernel". Edit config.txt and remove kernel= and initramfs.

This install process is very similar to the kernel package from the original Raspberry PiOS packages. It uses dpkg-divert "hack" to unpack the files, and then move the files to /boot/firmware.
