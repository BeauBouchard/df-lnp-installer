
Lazy Newb Pack Linux V0.40.04
-------------

I have assembled a small package to get people started on linux using the LNP interface and Dwarf Therapist updated to v0.40.04

You can download the package at: 

Included Mods
-------------
* Lazy Newb Pack for Linux 0.5.3-SNAPSHOT-20130822
* Utilities:
* Dwarf Therapist v23 (splintermind, pulled and built from source) with manual updated to v0.40.04
* Soundsense r42
* qfconvert 2.04
* chromafort 2010-04-25
* DF Announcement Filter 1.01
* Tilesets
    - [16x16] Phoebus v0.40.04

    
DF 40.04 Release notes:
-------------
* This is mainly another crash-fix release, though I was able to handle some other problems as well. I'm still hoping to get to optimizations (for the third time in these release notes!), but as usual that depends on stability. As you'll note below, a few of the older bugs are gone -- as we continue in this process, I'll work fixes for old bugs into the mix.
* Major bug fixes
* Fixed a crash with pathing for jumps
* Fixed a crash related to invading squads attempting to train
* Fixed an overpopulation bug for civilized critters and a related one for site animals
* Fixed problem with retired fort uniform settings crashing later visits to the fort
* Stopped a crash associated to misplaced books/slabs (root cause remains, added some logs)
* Fixed position appointment issue that caused some instability
* Tried to make idle code somewhat better about climbing while still getting dwarves out from being stuck
* People with a weapon should use it with the proper frequency now
* Other bug fixes/tweaks
* Fixed problem with animal training/taming vs. lingering combat data (caused job cancel spam and inability to complete jobs)
* Stopped nearby objects from being teleported by construction removal and a related problem with the item loop (ag/Quietust)
* Made site finder properly indicate flux layers (Quietust)
* Made game better respect existing directory structure in data/save when creating new directories
* Made tops of walls appear properly when trees above walls are removed
* Made strangulation take less time
* Enhanced sapling survivability
* Fixed a problem that caused vermin to occasionally be generated out of the loaded area
* Fixed a problem that corrupted the information about items on the ground with temperature changes
* Fixed some brokenness with climbing AI vs. ledge tops
* Fixed a broken instance of chasing opponent AI vs unwalkable spaces
* Made climbing have a higher path cost
* Made people less likely to climb after a failure
* Babies don't start strapped with a knife

  System Requirements
-------------

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

 Usage
=====

```
Usage: sudo ./startlnp
```

Tested On
=========
* Ubuntu 14.04 "Trusty Tahr"      fresh install.

