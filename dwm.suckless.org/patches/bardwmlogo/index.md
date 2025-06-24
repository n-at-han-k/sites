bardwmlogo
==========

Description
-----------
This patch add dwm logo before tags on the left side of the status bar for aesthetic or branding purposes.

* Introduces a new `DwmLogo` struct to store rectangle dimensions for the logo's strokes.
* Defines a fixed logo width (`dwmlogowdth = 54`) and shifts tag drawing accordingly to avoid overlap.
* Draws a dark background rectangle to distinguish the logo area visually.
* Renders the logo using several rectangles `drw_rect()` to form the characters "dwm" in a pixel-art style.

This patch is entirely visual and does not affect DWM's core functionality or performance. It can be useful for users who want a more personalized or distinctive look to their window manager.

![bardwmlogo_1 screenshot](bardwmlogo_1.png)

Download
--------
* [dwm-bardwmlogo-6.5.diff](dwm-bardwmlogo-6.5.diff) (2024-03-19)

Authors
-------
* Rizqi Nur Assyaufi - <bandithijo@gmail.com> (6.5)
