# FreeEMS Quick Start

TODO: Write scripts!

This project contains just a few files and aims to get you up and running ASAP
on a Debian based GNU/Linux system. The two files are this readme and a script
to get various things that you will need. It assumes that you have none of the
required items and will download and install everything that is needed to get
going in one big download session. Exactly how long that takes will depend on
the speed of your internet connection and computer hardware.

### But I Don't Have Debian

That's OK, the process is similar on other GNU/Linux systems too. If you have
Ubuntu you really just have a modified version of Debian anyway; it should work.
Other systems are similar enough to use this script with minor changes. For Mac
and Windows you can use the script as a guide on what you need to get and do.

### What You Will Get

The first step is to prepare your machine with the necessary and recommended
tools for each aspect of the project. The tools that this will get you are
listed below. If you already have some, edit the script before running it.

 1. Git version control software
 2. GCC/Binutils firmware tools
 3. Java JDK for OpenLogViewer
 4. Maven 3 for OpenLogViewer
 5. Dependencies for MegaTunix
 6. Other misc build tools (make, bc, etc)
 7. Other misc user tools (kdiff3, cutecom, etc)

The second step is to get all of the sources for each aspect of the project and
build them. The following projects will be pulled down and have useful sources
added for future reference.

 1. FreeEMS-Vanilla firmware source
 2. FreeEMS-Loader utility source
 3. MegaTunix tuning app source
 4. OpenLogViewer analysis app source
 5. FreeTherm thermistor curve app source
 6. Lacerated Pempheridae testing app source
 7. FreeEMS official documentation source 
 8. binflogger log recording tool source
 9. Likely other things too!

### Warning To Non-Noobs

This script assumes you have no idea how to do anything and attempts to do
everything for you. If you're a confident Linux user, you're not going to like
some of the things that it does. It could still be useful for you, however, so
you may like to edit out the clearly marked offending parts and then use it.

### Files And Dirs Created

 - /usr/local/maven3
 - /usr/local/maven (symlink)
 - ~/bin/
 - ~/workspaces/freeems/

### Modifications To Files
 
The following entries will be appended to your path variable in your .bashrc

 - ~/bin/
 - ~/workspaces/freeems/freeems-vanilla/bin/
 - ~/usr/local/maven/bin

The FreeEMS build tools repository will be added to your apt source list file.

 - /etc/apt/sources.list
 
Additionally Maven and Java related entries will be appended to your .bashrc

Finally, MegaTunix installs its files in your system directly. If you don't
like the idea of that, it has a debian build directory that you can use to
create a .deb file for installation in the usual way.

### Future Ideas

 - Make the script robust, for example test for stuff already installed/downloaded
 - Make the script ask the user for some things before installation
 - Make the script able to update itself and the entire source/project structure
