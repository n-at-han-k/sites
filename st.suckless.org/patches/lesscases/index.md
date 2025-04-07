lesscases
=========

Description
-----------
If you ever look at `x.c` and `config.def.h`, you'll see that the cursor shape
numbers are not sequential in `config.def.h`, and there are empty cases in the
cursor drawing code in `x.c`. This patch simply removes the empty cases and makes
the cursor shape numbers sequential.

Download
--------
* [st-lesscases-20250404-98610fc.diff](st-lesscases-20250404-98610fc.diff)

This patch embeds the customcursor patch.

* [st-lesscases-customcursor-20250405-98610fc.diff](st-lesscases-customcursor-20250405-98610fc.diff)

Authors
-------
* Mertoalex Ashley - <mertoalex+suckless@disroot.org>
