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

1. Settings > Cards > **Add card**. Give it a name such as "GSPro" and choose a picture.
2. On **Programs to open**, choose the GSPro with ProTee AutoStart recipe and browse to ProTee AutoStart's program.
   Its one open step uses **Arguments** `/run` (skips AutoStart's 5-second countdown), **Wait for** `GSPro`, and
   **Timeout (s)** `660` (AutoStart gives up after 600 seconds; this allows a minute more). Do not add another open
   step for ProTee Labs or GSPro when AutoStart already opens them.
3. On **Programs to close**, keep GSPro, `GSPconnect`, ProTee Labs and AutoStart in the closing group. Use
   **Learn by opening this card...** to review anything else this bay starts. `GSPconnect` has the window title "ProTee United VX"; if
   it stays open, ProTee Labs can think GSPro is still running on the next launch.
4. Check the ender choices. Exiting GSPro should finish the session; if exiting ProTee Labs is also meant to end it,
   make it an ender too. Keep the connector and any short-lived helpers as close-only rows.
5. **Review and try it** > **Try this card...**, then finish the test and **Save card**.

A working close list looks like: `GSPro, GSPconnect, ProTee Labs, ProTeeAutoStart`. If AutoStart runs as an AutoHotkey
script, it shows as AutoHotkey (for example `AutoHotkey64`) instead.

## Check it

Expect **Opening GSPro**, then the GSPro window. Check the ProTee connection and reach the range yourself: a window
wait does not check those. Quit GSPro normally and check that the connector, ProTee Labs and AutoStart close too.
Open again and quit ProTee Labs if you made it an ender. Finally open again, press the back-to-games button and
choose **Yes, end it**. Each route should bring the cards back, and the next launch should work without clearing
leftovers by hand. Leave the card unchanged if a known working bay uses a different program name; check its actual
programs before changing it.

---
BayLauncher owner guide, version 2026-10-27 (BayLauncher 1.0.4). © 2026 BA Custom Products LLC.
