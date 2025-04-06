lesscases
============

Description
-----------
If you ever looked `x.c` and `config.def.h`, you'll see that cursor shapes' numbers are not sequence in `config.def.h` and there's empty cases in `x.c`'s cursor drawer, that patch just deletes them and makes cursor shapes' numbers sequence.

Download
--------
* [st-lesscases-20250404-98610fc.diff](st-lesscases-20250404-98610fc.diff)

With customcursor
-----------------
This patch isn't compatible with customcursor patch so i combined them so if you want to use customcursor with this patch, just use this:

* [st-lesscasesandcustomcursortogether-20250405-98610fc.diff](st-lesscasesandcustomcursortogether-20250405-98610fc.diff)

Authors
-------
* Mertoalex Ashley - <mertoalex+suckless@disroot.org>
