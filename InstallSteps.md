# Installation #

This document shows you how to install Gswitch, start Gswitch automatically on every login and how you can easily add more background images.


## Package installation ##

Gswitch has the following package dependencies:
  * libgnome2-gconf-perl
  * libxml-simple-perl

You can install these via either synaptic or apt-get.


### Install from deb ###

If you are using Ubuntu or Debian Linux, you can download and install the Gswitch debian package.

This can be installed as follows:

`dpkg -i gswitch.deb`


### Install from source ###

You can also download the source and install it yourself. Simply copy all of the source directories from that tar.gz, or only copy the actual program, as shown here:

`tar zxf gswitch_src.tar.gz`

`cp -v gswitch/usr/bin/gswitch /usr/bin/`

`chmod +x /usr/bin/gswitch`


## Installing Gswitch ##
This step ensures that Gswitch runs automatically at every login.

### Step 1 ###
On your GNOME desktop, goto: System > Preferences > Startup Applications.

![http://gswitch.googlecode.com/svn/wiki/session1.jpg](http://gswitch.googlecode.com/svn/wiki/session1.jpg)

### Step 2 ###
Click on "Add".

![http://gswitch.googlecode.com/svn/wiki/session2.jpg](http://gswitch.googlecode.com/svn/wiki/session2.jpg)

### Step 3 ###
Type the following into the appropriate boxes, as detailed below:
  * Name: Gswitch
  * Command: /usr/bin/gswitch -t 30

**Please note that if you want your background to change more or less frequently, you should adjust the "30" to the number of minutes you want. For example, if you want the desktop background to change only once per hour, put 60 here. Likewise, if you want it to change every quarter hour, put 15.**

If you want gswitch to wait 60 seconds when it starts (before doing anything else), add the "-p" flag to the command above. This delays gswitch from loading a new background when it is started and is most useful when starting a new GNOME session on slower hardware. The above would become:
  * Command: /usr/bin/gswitch -p -t 30

![http://gswitch.googlecode.com/svn/wiki/session3.jpg](http://gswitch.googlecode.com/svn/wiki/session3.jpg)


## Adding more backgrounds ##
This section shows you how to add more backgrounds.

### Step 1 ###
On your GNOME desktop, goto: System > Preferences > Appearance.

![http://gswitch.googlecode.com/svn/wiki/background1.jpg](http://gswitch.googlecode.com/svn/wiki/background1.jpg)

### Step 2 ###
Click on the "Background" tab.

![http://gswitch.googlecode.com/svn/wiki/background2.jpg](http://gswitch.googlecode.com/svn/wiki/background2.jpg)

### Step 3 ###
Click on "Add" and browse to the image you want to include. Don't forget to set the right style for your image (one of: Tiled, Zoom, Centered, Scaled and Fill).
**Please note that newly added backgrounds won't be shown until your next login.**

![http://gswitch.googlecode.com/svn/wiki/background3.jpg](http://gswitch.googlecode.com/svn/wiki/background3.jpg)