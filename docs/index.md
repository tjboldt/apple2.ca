# Terence J. Boldt's Apple II site

## Projects

All my Apple II projects are now available on GitHub.

### Apple2-IO-RPi

This project provides I/O for an Apple II series 8 bit computer via a Raspberry Pi Zero W which is powered by the Apple II expansion bus. This includes using the attached RPi Zero W for it's storage, network and processor to provide new functionality for the Apple II.

Some of the features include:

1. Boot message which waits for RPi to be ready
2. ProDOS bootable drive from image stored on RPi
3. Execute Linux bash shell on the RPi from the Apple II
4. Load binary files directly from the RPi to the II
5. Update Apple II firmware in place from image on RPi
6. Supports two drive images at the same time (Note: backward compatible with previous firmware but requires firmware update in order to work with two drives)
7. Supports "RPI" command from BASIC to execute Linux commands from the command prompt or inside BASIC programs: `10 PRINT CHR$(4);"RPI ls -al /"`


[Apple2-IO-RPi](https://github.com/tjboldt/Apple2-IO-RPi)

### ProDOS ROM-Drive

This is a peripheral card for the Apple ][ series computers that acts as a read-only solid state disk drive (SSD) all in EPROM. Although it won't run DOS, it is fully ProDOS compatible and will appear as a read-only hard drive even when booting from another drive. It holds 1024 KB of disk data with the 256 byte firmware stored in block 0001 where the SOS boot loader normally resides. The drive boots ProDOS and into BASIC in under 1.5 seconds.

[ProDOS ROM-Drive](https://github.com/tjboldt/ProDOS-ROM-Drive)

### ProDOS-Utilities

This project is just starting but is intended to be both a command line tool and library to provide access to ProDOS based hard drive images. It is written in Go to be cross platform (Linux, Windows, macOS etc.). Functionality, naming and parameters are subject to change without notice. This project was started so I would be able to automate writing the firmware file into the drive image for building the Apple2-IO-RPi project. 

[ProDOS-Utilities](https://github.com/tjboldt/ProDOS-Utilities)

### Serial Virtual Drive

Also known as Virtual Serial Drive.

This creates a virtual drive over the serial port on an Apple II computer where the drive data is hosted by another PC. I wrote this in one weekend back in 2001 out of necessity. I was the final Apple II librarian for L.O.G.I.C.'s shareware collection and wanted to preserve the disks from the 1980's before they became unreadable. At the time, I made it work with just an Apple IIgs as it had a built-in serial port. Years later, others discovered the code on my website and it was improved and used in many other projects. This code repo is not maintained and only posted here for historical purposes.

[Serial Virtual Drive](https://github.com/tjboldt/Serial-Virtual-Drive)
