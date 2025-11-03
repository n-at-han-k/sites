Visual Unlock + DPMS
====================

Description
-----------
This patch keeps the screen unlocked but keeps the input locked.
That is, the screen is not affected by slock, but users will not
be able to interact with the X session unless they enter the correct
password.

Unlike the unlock screen patch, this uses an arg (-u) to enable the
unlocked screen functionality, and the mouse will remain hidden. The
primary use case for this would be in a script to spawn a screensaver
when the screen is locked.

The DPMS patch is also included, with a separate DPMS sleep timer in
config.def.h. This might be used to keep the screensaver on for 5
minutes, while running slock without -u has the screen sleep after 3
seconds of inactivity.

If you would not like to use DPMS, set both DPMS timers to 0 in your
config.h.


Download
--------
* [slock-visual-unlock-dpms-1.6.diff](slock-visual-unlock-dpms-1.6.diff)

Authors
-------
* cat <cat@plan9.rocks>
