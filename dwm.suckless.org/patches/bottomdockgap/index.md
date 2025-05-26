bottomdockgap
=======

Description
-----------
This patch adds a dedicated, respected area below all tiled windows for a dock.
This has been tested with plank and using the plank setting application
to configure plank to be at the bottom.  The height of the of the dedicated area
is configured by the static const unsigned int bottom_gap.  You set this to the number 
of pixels you want left at the bottom of the screen.

	static const unsigned int bottom_gap = 45;  // Adjust gap size here


This change will still allow backgrounds to be set by feh.  Plank will have to
be started in whatever way you chose to start other progams.

If you use this with picom, setting the borderpx = 0 will remove line artifacts left by plank.

Download
--------
* [dwm-bottomdockgap-6.4.diff](dwm-bottomdockgap-6.4.diff) (1.3k) (2025-05-25)


Author
------
* scf - <stevencfuchs@icloud.com>
