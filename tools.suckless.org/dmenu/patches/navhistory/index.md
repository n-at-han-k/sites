navhistory
==========

Description
------------
This patch provides dmenu the ability for history navigation similar to that
of bash. Press alt+p for the previous history and alt+n for the next.

Configuration
-------------
Set the maximum number of histories with a new variable 'maxhist' in config.h.
By default, it only records a new history if it is not the same as the last one.
To change this behaviour, set 'histnodup' to 0 in config.h.

Download
--------
* [dmenu-navhistory-5.0.diff](dmenu-navhistory-5.0.diff)
* [dmenu-navhistory-4.6.diff](dmenu-navhistory-4.6.diff)

### With Search
This patch extends navhist with history-search functionality. Press
ctrl-r, like in bash or ksh, and the suggestions will be replaced with
the history. Press ctrl-r again to revert.

* [dmenu-navhistory+search-20200709.diff](dmenu-navhistory+search-20200709.diff)
* [dmenu-navhistory+search-20250328-52fc8a0.diff](dmenu-navhistory+search-20250328-52fc8a0.diff) (2025-03-28)

Author
------
* phi <crispyfrog@163.com>
* Philip K. - philipk (at) posteo (dot) net
* [El Bachir](https://github.com/elbachir-one) (2025-03-28)
