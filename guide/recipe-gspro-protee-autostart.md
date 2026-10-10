[BayLauncher](../README.md) > Recipe: GSPro with ProTee AutoStart

# Recipe: GSPro with ProTee AutoStart

For bays with a ProTee VX that start GSPro through ProTee Labs. ProTee AutoStart is a free BA Custom Products tool that
clicks through ProTee Labs and GSPro to the range by itself:
[Protee-VX-Gspro-Smart-Start-up on GitHub](https://github.com/DiyGolfGuy/Protee-VX-Gspro-Smart-Start-up).

## Before you start
- GSPro opens normally from ProTee Labs on this PC.
- ProTee AutoStart is installed. Turn off its own "start with Windows" option, and in Task Manager > Startup apps
  disable it, so it only runs when the card starts it.
- Neither ProTee Labs nor GSPro is set to "Run this program as an administrator" (right-click the program > Properties >
  Compatibility). BayLauncher cannot close a program that runs as administrator.

## The card
1. Settings > Cards > **Add card**. Name it (for example "GSPro") and choose a picture.
2. Open step 1: **...** to ProTee AutoStart's program. **Arguments**: `/run` (skips its 5-second countdown).
   **Wait for**: `GSPro`. **Timeout (s)**: `660` (AutoStart gives up after 600 seconds; this allows a minute more).
3. **Save card**, then **Learn...**: start, wait until GSPro is fully in the range, **Done**. Keep ProTee Labs, GSPro
   and AutoStart ticked, untick anything else, and save.
4. Add `GSPconnect` to the close list if Learn did not list it. GSPro starts it (its window is "ProTee United VX"). If
   it stays open, ProTee Labs thinks GSPro is still running and will not open it the next time.

A working close list looks like: `GSPro, GSPconnect, ProTee Labs, ProTeeAutoStart`. If AutoStart runs as an AutoHotkey
script, it shows as AutoHotkey (for example `AutoHotkey64`) instead.

## Check it
Click the card: "Opening GSPro" shows, then GSPro comes up in the range. Press the back-to-games button and choose
**Yes, end it**: everything on the list closes and the cards come back. Do it twice.

---
BayLauncher owner guide, version 2026-10-07 (BayLauncher 1.0.2). © 2026 BA Custom Products LLC.
