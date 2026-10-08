[BayLauncher](../README.md) > Recipe: TruGolf Multisport

# Recipe: TruGolf Multisport

For TruGolf's E6 Product Launcher, where each sport is its own program. Leaving a sport (Exit Game) should go back
to the launcher's menu, and only closing the launcher should bring the cards back.

## The card
1. Settings > Cards > **Add card**. Name it (for example "SPORTS") and choose a picture.
2. Open step 1: **...** to E6 Product Launcher. **Wait for**: `E6 Product Launcher`.
3. **Close list**: `E6 Product Launcher` plus the program name of every sport you offer (see below).
4. **Game ends when these close**: `E6 Product Launcher`.
5. Optional: tick **When the game ends, also close any other program that opened during the game**, so a sport whose
   name is missing from the list still closes.
6. **Save card**.
7. Settings > General > **Seconds a program gets to close before it is forced**: `30`, then **Save**. This gives the
   launcher time to shut down by itself. TruGolf keeps its license on the PC, and a launcher that is forced closed
   too early can lose it (you would then have to unbind and activate it again with TruGolf).

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
Open the card, start a sport, use Exit Game: you are back in the launcher's menu. Close the launcher: the cards come
back. Start a sport again and use the back-to-games button: everything closes and the cards come back.

---
BayLauncher owner guide, version 2026-10-07 (BayLauncher 1.0.1). © 2026 BA Custom Products LLC.
