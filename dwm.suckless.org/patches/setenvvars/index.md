Set environment variables
=========================

Description
-----------
Allow setting environment variables inside `config.h`. This is a port of the dwl patch [setupenv](https://codeberg.org/dwl/dwl-patches/src/branch/main/patches/setupenv) to dwm.

Download
--------
* [dwm-setenvvars-6.5.diff](dwm-setenvvars-6.5.diff)
* Users of autostart patches might need to make sure their autostart function inside main() is started after setenvvars().

Authors
-------
* [notchoc](https://codeberg.org/notchoc) (original patch)
* [tch69](https://github.com/tch69) (dwm port)
