<img width="75" height="92" alt="image" src="https://github.com/user-attachments/assets/2330e67f-d0fc-44cd-9c08-42a6cd629307" />

# Debian-GNU-Linux-16-bit-PC-8086-
This Is Debian GNU/Linux on 16-bit Machines based on ELKS

Installation

Build ELKS images
On a modern Linux machine
git clone https://github.com/jbruchon/elks.git
cd elks
make

Write floppy image

    Insert a real floppy disk.

    Use dd to write the image:

    sudo dd if=elks.img of=/dev/fd0 bs=512

Boot hardware from floppy

    Insert the floppy into your vintage PC.

    Power on; ELKS should boot into its shell.

    Login as root (no password).

Install to HDD

    Partition the HDD using DOS tools or ELKS utilities.

    Format with FAT or MINIX (mkfs.minix).

    Copy ELKS system files from floppy to HDD.

    Adjust boot sector or use a bootloader (ELKS includes simple boot code).

    Reboot with HDD as primary boot device.


Login as root then vi /etc/issue Then Change ELKS 0.7.0 To Debian GNU/Linux then esc then :wq
