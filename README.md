Lazy Newb Pack Linux
====================
As of 2014-06-24, [the master repository](https://github.com/andrewd18/df-lnp-installer) is unmaintained. See [this post for more
information](http://www.bay12forums.com/smf/index.php?topic=130792.msg5403952#msg5403952). 

Overview
========

df-lnp-installer is a shell script that installs the Dwarf Fortress Lazy Newb Pack. It downloads and builds a DF installation from available source code and binaries. 

This is an attempt to update [andrew18's](https://github.com/andrewd18/) package assembler to DF 2014. Due to the rapid pace that Dwarf fortress is being updated at this time development is hard and many features will be missing or disabled until there is a lul an development. Untill then please feel free to check out the pre-assembled packages. 


Packages
-------------

There are several preassembled packages which can be downloaded for Dwarffortress V0.40.09

V0.40.09
-------------

Download it at : http://dffd.wimbli.com/file.php?id=8936




Included Mods
-------------

* Lazy Newb Pack for Linux 0.5.3-SNAPSHOT-20130822
* SoundSense r42 (app only, run update on first run)
* Dwarf Therapist v23.2 (splintermind, pulled and built from source) with manual
* Quickfort 1.01
* Chromafort 2010-04-25
* A series of blueprints for Quickfort.
* Various embark profiles.
* Tilesets
  - [16x16] Phoebus 0.40.04v01


System Requirements
===================

* A Java runtime environment for the LNP GUI.
* SDL 1.2, 32-bit
* LibGLU 1, 32-bit
* LibGTK 2.0, 32-bit
* OpenAL 1.2, 32-bit
* LibJPEG 6.2, 32-bit
* Git
* Mercurial (hg)
* Qt4 Development Libraries including qmake
* Python 2.x (for Quickfort)
* The following fairly standard Linux utilities:
  - wget
  - sha1sum
  - sed
  - tar
  - unzip
  - unrar
  - make
  - g++
  - gcc
  - xterm

The df-lnp-installer script will automatically check your system for the required libraries.

The Debian and Ubuntu command to install these dependencies is:
```
sudo apt-get install default-jre libsdl1.2debian:i386 libsdl-image1.2:i386 libsdl-ttf2.0-0:i386 libglu1-mesa:i386 libgtk2.0-0:i386 libopenal1:i386 libjpeg62:i386 git mercurial libqt4-dev qt4-qmake wget coreutils tar unzip make g++ gcc patch xterm sed python bzip2
```

The Fedora command to install these dependencies is:
```
sudo yum install java-1.7.0-openjdk gcc gcc-c++ automake libgcc.i686 git cmake glibc-devel.i686 zlib-devel.i686 perl-XML-LibXSLT perl-XML-LibXML mercurial qt.i686 libgcc.i686 qt-devel SDL.i686 SDL_image.i686 SDL_ttf.i686 gtk2.i686 mesa-libGLU.i686 openal-soft.i686 libsndfile.i686 xterm unrar unzip python
```

Usage
=====

```
Usage: df-lnp-installer.sh [OPTIONS]

Options:
--override-user-agent  # Download files as Mozilla user agent, not Wget user agent. Useful if you get 403 errors.
--skip-download        # Install using the existing contents of the ./downloads folder.
--skip-deps            # Install without checking for dependencies.
--skip-sha             # Install without checking file checksums.
--use-free-libs        # Force to use free graphic libs to solve "Not found" errors of DF.
--upgrade, -u          # Upgrade an existing DF installation.
--version, -v          # Print the df-lnp-installer version.
--help, --usage        # Print this message.
```

Full Installation
=================

1. Clone the git repository with `git clone https://github.com/BeauBouchard/df-lnp-installer.git`
2. Run `./df-lnp-installer.sh` and follow the prompts.
3. Once DF is installed, enter the DF folder and run ./startlnp.
4. Start the SoundSense r42 utility from the Utilities tab.
5. Click the "Pack Update" tab.
6. Click "Start Automatic Update".
7. Get a Dwarven Ale; it's going to be a while.
8. Once finished, close SoundSense, and muck about with LNP as normal.

Upgrading an Existing Installation
==================================

1. Update your git repository with `git pull`
2. Run `./df-lnp-installer.sh --upgrade`. When asked, enter the directory you already installed DF into.
3. Your save files and soundsense audio packs will be backed up.

Common Issues
=============
See [the WIKI](https://github.com/andrewd18/df-lnp-installer/wiki).


Tested On
=========

* Ubuntu 14.04 "Trusty Tahr"      fresh install.
