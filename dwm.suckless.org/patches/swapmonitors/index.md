# monitors

## Description

This patch adds the ability to swap tagsets and clients between monitors in dwm.
It helps users who use multiple monitors to quickly rearrange workspaces by moving
all windows and tag assignments from one monitor to another.

## Usage

After applying the patch, the following key binding will be available by default:

MODKEY + Shift + Apostrophe (')

This keybinding will:

- Swap the currently active monitor's tagset with the adjacent monitor's tagset.
- Move all clients (windows) between the two monitors, effectively swapping their contents.

> You can modify the keybinding by editing the following line in `config.def.h`:
>
> ```c
> { MODKEY|ShiftMask, XK_apostrophe, swapmon, {0} },
> ```

## Download

- [dwm-swapmonitors-20250510-cfb8627.diff](dwm-swapmonitors-20250510-cfb8627.diff)

## Author

Jameel Sawafta <jameelhsawafta@gmail.com>
