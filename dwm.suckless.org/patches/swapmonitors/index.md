swapmonitors
============

Description
-----------

This patch adds the ability to swap tagsets and clients between monitors in dwm.
It is particularly useful for users with multiple monitors who want to quickly
rearrange workspaces by moving all windows and their tag assignments from one
monitor to another.

#### Usage

After applying the patch, the following key binding is available by default:

**MODKEY + Shift + Apostrophe** (')

This keybinding will:

- Swap the currently active monitor's tagset with that of the adjacent monitor.
- Move all clients (windows) between the two monitors, effectively swapping their contents.

> You can customize this keybinding by modifying the following line in `config.def.h` file:
>
> ```c
> { MODKEY|ShiftMask, XK_apostrophe, swapmon, {0} },
> ```

Download
--------
* [dwm-swapmonitors-20250509-4cd2832.diff](dwm-swapmonitors-20250509-4cd2832.diff)

Author
------
* Jameel Sawafta - <jameelhsawafta@gmail.com>
