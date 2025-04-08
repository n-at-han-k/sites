floatingstatus
==============

Description
-----------
This patch allows you to transform the status bar into a floating bar, with
customizable height, as well as vertical and horizontal padding.

[![screenshot.png](screenshot.png)](screenshot.png)

#### Config

Everything is in `config.def.h`
* `barpadv`   - [int]  Vertical padding: how far the bar is from the top.
* `barpadh`   - [int]  Horizontal padding: how far the bar is from each side.
* `barheight` - [int]  Bar height: How long the bar is vertically.
* `floatbar`  - [Bool] Whether to show or hide the bar.

Download
--------
* [floatingstatus-20250408-cfb8627.diff](floatingstatus-20250408-cfb8627.diff)

Authors
-------
* Abhinav Prasai - <abhinav.prsai@gmail.com>
