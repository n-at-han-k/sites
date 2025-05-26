bottomdockgap
=============

Description
-----------
This patch adds a dedicated, reserved area below all tiled windows for a dock.

It has been tested with Plank, using the Plank settings application to configure
the dock position at the bottom of the screen. The height of this dedicated area is
controlled by the static constant `bottom_gap`.
You can set this value to the number of pixels you want to reserve at the bottom.

```sh
static const unsigned int bottom_gap = 45;  // Adjust gap size here
```

This change still allows backgrounds to be set using `feh`. Plank must be started
manually or through your preferred startup method.

If you use this patch with Picom, setting `borderpx = 0` will remove line artifacts caused by Plank.

Download
--------
* [dwm-bottomdockgap-6.4.diff](dwm-bottomdockgap-6.4.diff) (1.3k) (2025-05-25)

Author
------
* scf - <stevencfuchs@icloud.com>
