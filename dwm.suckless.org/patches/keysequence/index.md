keysequence
===========

Description
-----------

This patch allows for defining sequential keybindings, for example `MOD+A W`.
This is done not through the `XGrabKey()` which is used for root bindings,
but by the `XGrabKeyboard()` so any key presses that are not defined will
stop the matching without passing them to programs. This behaviour is
less confusing.

It defines new bindable function `keypress_other()` that as argument takes
a pointer to array of bindings.

    static Key keyseq_a[] = {
        { 0,	        XK_t,	setlayout,	    {.v = &layouts[0]}},
        { ShiftMask,	XK_t,	setlayout,	    {.v = &layouts[1]}},
        { MODKEY,		XK_y,	setlayout,	    {.v = &layouts[2]}},
        {0}
    }

    static Key keys[] = {
        { MODKEY,       XK_a,   keypress_other, {.v = keyseq_a}},
        {0}
    }

This assigns `MOD+a t`, `MOD+a T`, `MOD+a MOD+y` to changing layout, you can
nest bindings endlessly.

Notice that now keybinding arrays are ended by `{0}` empty element,
this is necessary because `Arg` structure can take only pointer
sized elements, there's no place to specify size so it has to be
calculated while running.

While typing sequence all events are ignored other than key presses
and mouse, moving mouse exits sequence.

Save your hands! Don't make long sequences, stick to simple, easy to
access binding and use plain letters, realistically speaking you'll
use it for dmenu scripts, layout bindings, and other rarely used
commands.

Download
--------
* [keysequence-20250606-0d6af14.diff](keysequence-20250606-0d6af14.diff)

Author
------
* TUVIMEN <hexderm@gmail.com>
