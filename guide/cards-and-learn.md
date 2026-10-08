[BayLauncher](../README.md) > Cards and Learn

# Cards and Learn

Each card is one game. Settings > **Cards** lists them in the order they appear.

## Open Settings
Click the lock button in the top-right corner of the cards screen, enter the staff PIN, and choose **Settings**.

## Make a card
1. **Add card**. Type the **Name on the card**.
2. **Choose picture...** for the card's picture. **Picture shape**: "Whole picture (black bars if needed)" shows all of
   it, which is best for pictures with text or a QR code; "Fill the card" crops the edges.
3. **Open steps (run in order)**: a new card already has one step. Press **...** on it to browse to the program
   (**Wait for** is filled in with the program's name). **Add step** adds another. **Arguments** only if the program
   needs them. **Wait for**: the program's name (without .exe) or words from its window title; the next step starts
   when that window appears. **Timeout (s)**: how long to wait for it. If it does not appear in time, BayLauncher
   closes what the card started and tries once more; after the second try it shows a problem.
4. **Save card**.

Use **Move up** and **Move down** to change the order, and **Delete** to remove a card.

## Learn: let BayLauncher find the programs to close
A game often opens more programs than the one you start (a launcher, a helper, a connector). They all need to close
when the game ends, and **Learn** finds them for you.
1. Save the card first, then press **Learn...**.
2. **1. Start the card**: BayLauncher notes what is already running, then starts the card.
3. Wait until the game is fully open (sign in or click through if it needs that), then press **2. Done**.
4. Helpers (crash reporters, set-up tools, updaters) are left unticked. Untick anything else that is not part of the
   game, then **3. Save as close list**.

## The close list and when a game ends
- **Close list**: the programs (names without .exe, separated by commas) that are closed when the game ends.
- When one of them closes (and it had a window), or the back-to-games button is used, all of them are closed and the
  cards come back.
- **Game ends when these close**: leave it empty for most games. For a launcher that opens separate games, put just
  the launcher here (see [Recipe: TruGolf Multisport](recipe-trugolf-multisport.md)).
- **When the game ends, also close any other program that opened during the game**: for launchers whose games have
  many different program names. Anything that was already open before the card was clicked is not closed by it.
- Some programs are never closed, even when they are on a close list: Windows' own programs (Explorer, Task Manager
  and everything in the Windows folder), command and PowerShell windows, Python programs, Microsoft Edge and
  WebView2, and programs that run as administrator.
- **Must be closed first**: programs that are closed (and confirmed gone) before the card starts.
- **Add from a folder...**: adds every program in a folder and its subfolders to the close list (for example a
  launcher's Products folder). Crash reporters, updaters and setup programs are left out. Check the list, then
  **Save card**.
- Programs get a few seconds to close by themselves before they are forced (Settings > General).

## Good to know
- Only put games and their own helpers on a close list. If a program on a card's list is already open with a window
  when the card is clicked, BayLauncher brings it to the front and treats it as the running game. Leftovers without a
  window are closed first and the card starts normally.
- Never put a firmware updater, a launch-monitor utility or a crash reporter (for example `UnityCrashHandler64`) on a
  close list.
- When a card is clicked, "Opening ..." shows until the game is up. There is no need to click again.

---
BayLauncher owner guide, version 2026-10-07 (BayLauncher 1.0.1). © 2026 BA Custom Products LLC.
