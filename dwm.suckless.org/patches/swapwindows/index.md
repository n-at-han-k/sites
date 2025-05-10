# swapwindows

## Description

This patch allows swapping the selected client (window) with the selected window
on the other monitor. Useful for moving a window to the other monitor while
preserving the window focus and order.

## Usage

After applying the patch, the following key binding will be available by default:

MODKEY + Shift + /

This keybinding will:

- Swap the currently focused window with the focused window on the next monitor (if any).
- If the other monitor has no selected client, it will just move the current focused window to it.
- Rearrange and refocus appropriately after the operation.

> You can customize this keybinding in your `config.def.h`:
>
> ```c
> { MODKEY|ShiftMask, XK_slash, swapwindow, {0} },
> ```

## Download

- [dwm-swapwindows-20250510-cfb8627.diff](dwm-swapwindows-20250510-cfb8627.diff)

## Author

Jameel Sawafta <jameelhsawafta@gmail.com>
