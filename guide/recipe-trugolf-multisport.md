[BayLauncher](../README.md) > Recipe: TruGolf Multisport

# Recipe: TruGolf Multisport

For TruGolf's E6 Product Launcher, where each sport is its own program. Leaving a sport (Exit Game) should go back
to the launcher's menu, and only closing the launcher should bring the cards back.

## The card

1. Settings > Cards > **Add card**. Name it (for example "SPORTS") and choose a picture.
2. On **Programs to open**, choose the E6 recipe and browse to **E6 Product Launcher**. The open step waits for
   `E6 Product Launcher`. Start only the launcher here; guests choose their sport from its menu.
3. On **Programs to close**, tick **Close** for `E6 Product Launcher` and every sport you offer (see below). Tick
   **Ends game** for **E6 Product Launcher only**. A sport ending must leave the launcher menu running.
4. Review any programs found by the recipe or **Learn by opening this card...**. Leave the wider **also close any other program** option
   off while you build and test the named group; it is not needed to close sports that are listed correctly.
5. **Review and try it** > **Try this card...**. Test a sport's **Exit Game**, the launcher closing, and the back button
   as described below. Finish the test, then **Save card**.
6. Check Settings > General > **Seconds a program gets to close before it is forced** is at least `30`. The E6
   recipe raises a shorter value to 30; it does not shorten a longer value. This is a setting for all cards. The
   sport closes first and the E6 launcher last, giving it time to finish its normal shutdown. TruGolf keeps its
   license on this PC; avoid forcing the launcher closed early. If its license needs recovery, follow TruGolf's
   unbind and activation process or contact BA Custom Products for help.

## Finding the sports' program names
1. Open File Explorer at `C:\Program Files\E6 Product Launcher\Products`. Each sport has its own folder.
2. In each sport's folder, the sport's program is a file of type "Application" (skip `UnityCrashHandler64` and any
   set-up or configuration tool). Its name without ".exe" goes on the close list (for example `Hoops`, `Cornhole`).
3. Sports installed separately (for example TruGolf's shooting games) live in their own folders under
   `C:\Program Files\TruGolf`. Add them the same way.

Never add: `CefSharp.BrowserSubprocess` (the launcher's built-in browser, which keeps you signed in; it closes with the
launcher), `UnityCrashHandler64`, `FirmwareUpdater` (closing it during an update can harm the device), set-up or
configuration tools, or anything from TruFlight utilities.

An example close list from a working bay: `E6 Product Launcher, E6MultiSport, MultiSport, Quarterbacks, Cornhole,
Field Goal Frenzy, Hoops, Inside Heat, WildWest, Wilderness Hunter`.

## Check it

Open the card, start a sport and use **Exit Game**: expect the launcher's menu, with no BayLauncher cleanup of that
menu. Close the launcher: expect the cards back. Start a sport again and use the back-to-games button: expect the
sport and its game helpers to close, then the launcher, then the cards. Open the card once more to check that it
starts normally and TruGolf's activation is still intact. A sport returning straight to the cards usually means
it was made an ender, or no explicit launcher ender was set.

---
BayLauncher owner guide, version 2026-10-27 (BayLauncher 1.0.5). © 2026 BA Custom Products LLC.
