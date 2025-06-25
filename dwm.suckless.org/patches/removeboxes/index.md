removeboxes
===========

Description
-----------
This patch removes boxes next to tags with windows in them as well
as the box indicating whether a tag has a floating window in it.

A vanilla dwm bar looks like this (also showcasing a tag with a floating
window in it):

![before applying removeboxes](dwm-removeboxes-before_patch.png)

And this is what it looks like after removeboxes is applied:

![after applying removeboxes](dwm-removeboxes-after_patch.png)

The patch is best used when combined with something like [underlinetags](https://dwm.suckless.org/patches/underlinetags/),
but it does work nicely when used just by itself.

Download
--------
* [dwm-removeboxes-6.5.diff](dwm-removeboxes-6.5.diff) (1.5K) (20250625)

Authors
-------
* Jakub Skowron <jakubskowron676@gmail.com>
