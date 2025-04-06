option
=========

Description
-----------
This patch adds variable called `option` to config.def.h so st can run shell with argument.


Example
-------
`static char *shell = "/usr/bin/ash";`

`char *option = "-l";`

so now st runs ash with `-l` argument so ash opens as login shell so it sources /etc/profile.d/ files.

[![ash-uses-profile.d-scripts](st-option-preview-grayscale.png)](st-option.png)

Download
--------
* [st-option-20250404-98610fc.diff](st-option-20250404-98610fc.diff)

Authors
-------
* Mertoalex Ashley - <mertoalex+suckless@disroot.org>
