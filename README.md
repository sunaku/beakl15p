# BEAKL-15p Keyboard Layout

This is a variation of [BEAKL]-15 that emphasizes programming comfort:

* Digits and shifts are standard (shifted comma isn't an exclamation).
* Comma and period are adjacent and in standard order (comma, period).
* Slash is on the home row for easy path separation and Vim searching.

[BEAKL]: https://deskthority.net/wiki/BEAKL

## Preview

Besides digits, only 3 keys have been moved: comma, period, and slash.

![Preview of this layout on a typical 60% keyboard](preview.png)

See [my Ergodox EZ config](
  https://configure.ergodox-ez.com/ergodox-ez/layouts/vKBnl
) for a more advanced example of this layout.

## Linux

Install:

    cat linux/usr-share-X11-xkb-symbols-us >> /usr/share/X11/xkb/symbols/us
    echo now please restart your X session

Activate:

    setxkbmap -layout us    -variant beakl15p         # one layout; no switch
    setxkbmap -layout us,us -variant beakl15p,basic   # dual layout switching
