customcursor
============

Description
-----------
This patch adds a constant value called `CUSTOM_BLOCK` to config.def.h to change snowman with custom cursor.


Example
-------
`static unsigned int cursorshape = 7;`

`#define CUSTOM_BLOCK 0x003B /* semicolon (U+003B) */`

[![custom-cursor-as-semicolon](st-customcursor.png)](st-customcursor.png)

Download
--------
* [st-customcursor-20250405-98610fc.diff](st-customcursor-20250405-98610fc.diff)

Authors
-------
* Mertoalex Ashley - <mertoalex+suckless@disroot.org>
