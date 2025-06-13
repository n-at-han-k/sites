gridall
========

Rationale
---------
Sometimes a window get lost in one of the tags and I just want to find it and focus on it, without changing its tag.

Description
-----------
This patch adds 2 new functions. One to view all windows in all tags (with the gaplessgrid layout) and another to view the selected window in the tag it is (with the monocle layout). The idea is to press a shortcut (for example Mod+g) to see all windows and, after selecting one, press another shortcut (for example Mod+r) to view that window in its tag.
The patch depends on 2 other patches: [gaplessgrid](../gaplessgrid) and [winview](../winview). I have included a patch to apply on top of a fork that already has these 2 patches (dwm-gridall-6.5.diff) and a patch that include all 3 patches: winview + gaplessgrid + gridall (dwm-winview+gaplessgrid+gridall-6.5.diff).
This patch also is an example of how to combine 2 functions in a single shortcut so an user can further customize their own dwm.

Download
--------
* [dwm-gridall-6.5.diff](dwm-gridall-6.5.diff)
* [dwm-winview+gaplessgrid+gridall-6.5.diff](dwm-winview+gaplessgrid+gridall-6.5.diff)

Authors
-------
* André Desgualdo Pereira - desgua `<desgua@gmail.com>`
