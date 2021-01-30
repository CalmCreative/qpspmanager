# Description
QPSPManager is a PBP File manager for Linux. It's intended to use as a user friendly GUI to the known tedious pack and unpack processes of the PSP PBP files, directory generation and further copy into the PSP, in order to execute those binary files in PSPs with firmware 1.50.

QPSPManager automates this process to make it a simple task to the end user, who will only have to select a PBP file and the PSP directory, leaving all other tasks to the program. It also provides some other cool features such as selecting custom PNG, PMF and AT3 files to use as an icon or background in the PSP menu.

QPBPManager also allows the user to backup the savegames to the computer and copy those savegames later to the PSP.

# Changes

Hi there! I'm just a guy that saw this ancient project and thought 'yeah, this is awesome but it could do with some work'.

What you see here was originally built to target qt4. As such, some functions (such as the applications manager) have functionality that is largely broken when targetting a greater version of qt. However, with a bit of work I managed to develop some light fixes that reinstate that functionality and also allow it to compile for newer versions of qt.

The downside to this is that video encoding *is broken* currently. As long as you do not desire to encode video, this little 'rebirth' should work fine. Compile it as you would normally, and all should be well.

Have fun.

CC

## Features

- Unpacks PBP files and selects automatically the icon and background files from the source file.
- Extracts the program name included in the PBP file and sets it as default output directory.
- Extracts the ELF of the PBP file and packs a fake PBP file without the ELF for showing in the menu of the PSP.
- Allows to select custom icon and background files to use in the menu.
- Allows to select custom video and music files to use in the menu.
- Allows to select the output directory on the PSP and the actual PSP directory, which is saved as an option for further usages, so you only have to configure it once (as long as the PSP directory does not change).
- Provides support for backup the savegames on the PSP to the computer and viceversa.
- Allows to compress ISO files to CISO files.
- Allows to expand CISO files to ISO files.
- Manages the ISO/CISO files on the PSP, allowing to delete them and copy them compressed or non compressed to the PSP.

# Installation
QT toolkit, g++ and zlib required.

    qmake
    make
    make install

# Legacy Website
http://qpspmanager.sf.net
