Squares
=======

Description
-----------
Instead of changing the color of the entire screen to indicate the current lock
state, draw centered squares on each monitor and change the square colors.

This patch requires xrandr to be active and otherwise defaults to the original
slock behavior.

Use `squaresize` in `config.def.h` to set the size of the square (in px).

Download
--------
* [slock-squares-1.5.diff](slock-squares-1.5.diff)

Apply the following patch on top of the previous one to ensure that the number
of squares matches the length of your current input for responsive behavior.

* [slock-squares-password-1.5.diff](slock-squares-password-1.5.diff)

Authors
-------
* bsuth - <bsuth701@gmail.com>
* Jack Avery - <jack.avery.business@gmail.com> (input patch)
