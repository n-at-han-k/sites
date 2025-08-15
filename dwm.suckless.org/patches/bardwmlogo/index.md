bardwmlogo
==========

Description
-----------
This patch adds a DWM logo to the left side of the status bar, positioned before
the tags, for aesthetic or branding purposes.

* Introduces a new `DwmLogo` struct to store the dimensions of the logo's strokes.
* Defines a fixed logo width (`dwmlogowdth = 54`) and adjusts tag rendering to prevent overlap.
* Draws a dark background rectangle to visually separate the logo area.
* Uses multiple `drw_rect()` calls to render a pixel-art style "dwm" logo using rectangles.

This patch is purely visual and does not impact DWM's core functionality or performance.
It may appeal to users who want a more personalized or distinctive appearance
for their window manager.

![bardwmlogo_1 screenshot](bardwmlogo_1.png)

Download
--------
* [dwm-bardwmlogo-6.6.diff](dwm-bardwmlogo-6.6.diff) (2025-08-15)
* [dwm-bardwmlogo-6.5.diff](dwm-bardwmlogo-6.5.diff) (2025-06-24)

Authors
-------
* Rizqi Nur Assyaufi - <bandithijo@gmail.com>
