setenvvars
==========

Description
-----------
Allows setting environment variables within `config.def.h`.
This feature is ported from the dwl patch [setupenv](https://codeberg.org/dwl/dwl-patches/src/branch/main/patches/setupenv).

Users of autostart patches should ensure that their autostart function
inside `main()` is called after `setenvvars()`.

Download
--------
* [dwm-setenvvars-6.5.diff](dwm-setenvvars-6.5.diff)

Authors
-------
* [notchoc](https://codeberg.org/notchoc) (original patch)
* [tch69](https://github.com/tch69) (dwm port)
