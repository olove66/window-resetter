# window-resetter

https://github.com/olove66/py-asciiquarium/

https://github.com/abishekvashok/cmatrix

https://github.com/busyloop/lolcat

https://github.com/aristocratos/btop

https://github.com/nicolargo/glances

https://github.com/dustinkirkland/hollywood

https://github.com/xorg62/tty-clock

https://github.com/joechiu/clock

```
import pygetwindow as gw

def adjust_to_screen(settings):
    for window, (left, top, width, height) in settings.items():
        hwnd = gw.getWindowsWithTitle(window)
        if not hwnd: continue
        hwnd = hwnd[0]
        hwnd.moveTo(left, top)
        hwnd.resizeTo(width, height)

home = dict(
    Outlook=(1910, 0, 1018, 1071),
)
adjust_to_screen(home)

tri_big_screens_0 = dict(
    Youtube=(-1456, 1550, 1459, 1049),
)
adjust_to_screen(tri_big_screens_0)

w = gw.getWindowsWithTitle("Outlook")[0]
w.box
# tuple(w.box)
```
