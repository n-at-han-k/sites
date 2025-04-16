dyn-battery
===========

Description
-----------
This patch implements a function that displays the status and capacity of
all present batteries (only supported for Linux).

The order of the format identifiers is hard-coded: battery number (%u),
state (%s), capacity (%s). Example:  
"[BAT%u: %s%s]" -> [BAT0: +58]

![Example](image.png)

Download
--------
* [slstatus-dyn_battery-20250416-f68f492.diff](slstatus-dyn_battery-20250416-f68f492.diff)

Author
------
* Madison Lynch <madi@mxdi.xyz>