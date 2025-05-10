swapwindows
===========

Description
-----------

This patch enables swapping the currently focused client (window) with the
selected window on another monitor.
It is useful for moving a window between monitors while preserving window focus
and layout order.

#### Usage

After applying the patch, the following key binding is available by default:

**MODKEY + Shift + /**

This keybinding will:

- Swap the currently focused window with the focused window on the next monitor (if one exists).
- If the other monitor has no selected client, it will simply move the currently
focused window there.
- Automatically rearrange and refocus windows as needed after the operation.

> You can customize this keybinding in your `config.def.h` file:
>
> ```c
> { MODKEY|ShiftMask, XK_slash, swapwindow, {0} },
> ```

Download
--------
* [dwm-swapwindows-20250509-00ea4c4.diff](dwm-swapwindows-20250509-00ea4c4.diff)

Author
------
* Jameel Sawafta - <jameelhsawafta@gmail.com>
