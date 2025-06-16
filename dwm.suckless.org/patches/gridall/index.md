gridall
=======

Description
-----------
This patch introduces two new functions:

1. One to view all windows across all tags using the gaplessgrid layout.

2. Another to view the selected window in its original tag using the monocle layout.

The idea is to press a shortcut (e.g., `Mod+g`) to display all windows, then after
selecting one, press another shortcut (e.g., `Mod+r`) to jump to that window's tag
and focus on it.

This patch depends on two other patches: [gaplessgrid](https://dwm.suckless.org/patches/gaplessgrid)
and [winview](https://dwm.suckless.org/patches/winview).

If you already have the other two patches added to your `dwm` build, you can simply
apply `dwm-gridall-6.5.diff`. If not, I've also created a combined patch
that includes winview, gaplessgrid, and gridall `dwm-winview-gaplessgrid-gridall-6.5.diff`.

Additionally, this patch serves as an example of how to combine two functions
under a single shortcut, allowing users to further customize their `dwm` setup.

**Note:** Sometimes a window may get "lost" in one of the tags. This patch helps
you quickly find and focus on it without having to move it or change its tag.

Download
--------
* [dwm-gridall-6.5.diff](dwm-gridall-6.5.diff)
* [dwm-winview-gaplessgrid-gridall-6.5.diff](dwm-winview-gaplessgrid-gridall-6.5.diff)

Authors
-------
* André Desgualdo Pereira - <desgua@gmail.com>
