# Linux Debian (.deb) package template

## Instructions

* Copy the directory template and rename it by replacing `VERSION` with the build date - eg. for a build made on Feb 26th 2015 the directory should be called `praxis-live_150226-1_all`
* Inside the new directory, edit the `DEBIAN/control` file, replacing VERSION - eg. Version: 150226-1 **Use an editor that doesn't create hidden backup files!**
* Copy the contents of the Zip distribution of Praxis LIVE into `usr/lib/praxis-live` - the Praxis LIVE launch script should end up at `usr/lib/praxis-live/bin/praxis_live`
* To build the .deb file, run `fakeroot dpkg-deb -b praxis-live_******-1_all` on the directory.
