#tinyCA2 - version 0.7.5-7
To be able to create certificate requests/certificates with utf8 support, add this lines to openssl.conf to [ req ] section

**
string_mask = utf8only
utf8 = yes
**

#tinyCA2 - version 0.7.5-3

This is a "fork" from debian sources.
* This repo contains shamelessly stolen debian patches (stolen-from-debian.patch). The debian patch has been modified to be used with arch linux.

* The package contains also 'fix-tinyca-paths.patch' and the modified PKGBUILD from arch aur repository. I'm not sure the author for fix-tinyca-paths.patch', but, the credits for the PKGBUILD must go to Marti Raudsepp <marti@juffo.org>

##My contribution to this package
* New github repo from debian's source
* Cleaned the debian patches by removing debian specific stuff
* PLGBUILD is avilaible at https://github.com/glennie/arch-pkgbuilds, in the tinyca2 sub directory

##Changelog
version 0.7.5-7 - Oct 09 2019
 * Added utf-8 support

version 0.7.5-2 - Tue May 31 2014
  * Added arch related stuff
  * Cleaned debian related stuff
  * Moved templates from /usr/share/tinyca2 to /etc/tinyca

version 0.7.5-3 - Sat August 29 2015
  * added patches sub dir currently used patches
    * Added sha2 support by a patch stolen from Debian bug tracking system (https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=759481#10). The patch is from Ross Vandegrift <ross@kallisti.us>

##Final words
* Give credit where credit is due : my own contribution here is very limited. Please go through the source and give credits to contributors.
* Tested on my arch installation. YMMV. It may eat your kitten, bite you dog or burn your cpu. So use this package at your own risk ;-)
