preview all windows
===================

Description
-----------
Allows you to preview all window image thumbnails under the current display,
and when clicked, it will jump to the corresponding application window.

[![preview all windows](preview-all-windows.png)](preview-all-windows.png)

I used two X11 extensions — XComposite's off-screen storage feature
and XRender — to capture the window image.

> [!WARNING]

> The project is still in development.

> If you're using patches like `actualfullscreen` or `awesomebar`, please uncomment
> the corresponding one in `config.def.h`.
```
#define ACTUALFULLSCREEN
#define AWESOMEBAR
```

Download
--------
* [dwm-preview-all-windows-6.5.diff](dwm-preview-all-windows-6.5.diff)

This patch is like the above, with keys to select windows in the preview.
`Mod + j`/`Mod + k` to setect a window, `Mod + Return` to open it.

* [dwm-preview-all-windows-20250407-e381933.diff](dwm-preview-all-windows-20250407-e381933.diff)

Authors
-------
* HJ-Zhang - <hjzhang216@gmail.com>
* El Bachir - <bachiralfa@gmail.com>
