[BayLauncher](../README.md) > Cards and Learn

# Cards and Learn

Each card is one game. Settings > **Cards** lists them in the order they appear.

## Open Settings
Click the lock button in the top-right corner of the cards screen, enter the staff PIN, and choose **Settings**.

## Before changing a working bay

End the running game first. Settings > Tools > **Export settings and pictures...** makes a portable copy of the
current setup. Keep it somewhere safe before making several changes. Adding or editing a card needs no internet.

## Make a card, one step at a time

Choose **Add card** to open the guided builder. **Next** moves through its four pages, **Back** lets you change an
earlier answer, and **Cancel** leaves the saved cards alone. **Help with this step** or F1 opens the current step's
help. **Open full card help** opens this chapter. Both work without an internet connection.

### Name and picture

Give the card a name guests will recognise. Choose a picture, or leave it empty to show the card's name.
**Show the whole picture** keeps text and QR codes visible; **Fill the card (crop the edges)** may crop them. The preview helps you
check the choice. These are draft changes until **Save card** succeeds.

### Programs to open

Choose **GSPro with ProTee AutoStart**, **TruGolf Multisport / E6 Product Launcher** or **Other program**, then
**Use this setup...** and browse to that program on this PC. Recipes are starting points: check all program locations
and the close group they suggest. Use **Other program** for one ordinary game or a different launcher, then add
its game-only helpers after reviewing Learn. A recipe cannot know which helpers your particular bay needs.
When editing a working card, keep its current programs unless you mean to replace the draft's open and close
choices with a new setup.

The guided builder uses installed `.exe` programs. If an existing recipe needs a script or Windows shortcut,
keep it in **Advanced launch and close settings** instead; choose its window wait and close names there yourself.

Put the open steps in the order they need to run with **Up** and **Down**. **Add another program...** adds a separate
open step; use it only for something the launcher does not start itself. **Arguments (optional)** are extra
instructions, such as AutoStart's `/run`; leave them empty unless the program needs them.

For **Other program**, the initial wait and close name come from the program you choose. If that program is only
a small starter for another game, change **Wait for** to the real game's window and add its actual program name
to the close group. A background utility with no visible window cannot satisfy a window wait.

Tick **Wait for a visible program window before continuing**, then enter **Program name or text in its window
title** and **Maximum wait in seconds**. These are called **Wait for** and **Timeout (s)** in the advanced editor.
The wait means a new visible window from a program that was not running when the card started. Use its program
name without `.exe`, or words in its window title. It does not check a launch-monitor connection, sign-in, course
loading or readiness to play. Untick the wait only when the next step can start immediately. On a startup failure,
the normal engine cleans up and tries once more; a wrong wait can therefore take about twice the timeout before
showing a problem.

### Programs to close

Review every row. **Close** puts that program in this game's closing group. **Ends game** makes closing
that program the signal to end the whole group and bring the cards back. Every ender must also have **Close**
ticked. Use actual program names, without `.exe`, rather than a shortcut's display name. **Add name** or
**Browse...** adds one. **Find programs in a folder...** offers unticked suggestions to review. **Learn by opening
this card...** can find programs the launcher starts for you; review the results before adding them to the draft.

With no explicit enders, any close-listed program that BayLauncher has seen with a window can end the group.
The GSPro and Other program recipes use this existing rule. If short-lived helpers should not end the game,
choose explicit enders such as GSPro and ProTee Labs, keeping the connector and AutoStart as close-only rows.
For E6 Multisport, only **E6 Product Launcher** is the ender: a sport's **Exit Game** must return to its menu.
Sports and other game helpers close before the E6 launcher; use at least 30 seconds of closing grace.
With no **Close** boxes ticked, the programs in the opening steps are still the fallback closing group.

Keep firmware updaters, maintenance/configuration tools, crash reporters, system or elevated programs and
unrelated background utilities out of the group. Leave wider **also close any other program** cleanup off unless
you deliberately need it. Recipes and Learn do not turn it on automatically.

### Review and try it

Check the name, picture, open steps, closing group and enders. **Try this card...** starts real programs with the
normal game engine. Check a normal quit, the back-to-games button, and a second launch. For E6, a sport's
**Exit Game** must leave its launcher menu open; ending the session closes the sport before the launcher.

A window appearing does not prove the game is connected or ready to play. Check that in the game yourself,
and read any problem reported by the test. Finish the test and close its game before saving. **Save card** applies
the draft only after validation and a successful settings save. **Cancel** leaves the saved cards unchanged.

## Edit, copy and undo

Select a card in Settings > Cards and choose **Edit with guide...** to use the same four pages for an existing
card. **Duplicate** opens a separate draft based on that card with a suggested new name; review its name and
settings before saving. Use **Move up** and **Move down** to change carousel order, or **Delete** to remove a card
after confirmation. Deleting a card does not uninstall its game.

You can also change the selected card's name and picture in Settings, or expand **Advanced launch and close
settings** for the original step grid and name lists. **Save card** applies those edits. If you move on with
unsaved edits, **Save** applies them first, **Discard** keeps the saved card, and **Cancel** keeps your edits open.
This choice also appears before starting Learn, a test or another guided edit.

**Discard edits** reloads the saved card and loses only the unsaved edits. **Undo last save** reverses the last
card save or addition made while this Settings window is open; undoing an addition removes that card. It restores
only that card, not global settings such as E6's longer closing grace. Save or
discard any current edits first. This one-step undo is cleared by deletion, reordering, external settings reload
or closing Settings. It is not a history of every change.

Card saves, deletion and reordering keep a previous-settings file in `C:\ProgramData\BayLauncher\backups`; the
newest 20 are kept. Settings > Tools > **Open data folder** lets you find them. They contain settings, not a
complete copy of the pictures. Use **Export settings and pictures...** for a full copy you can import through
Tools. Ask BA Custom Products for help with a settings-only backup rather than guessing which file to replace on
a working bay. A failed save leaves the previous configuration in use and keeps the edits available to correct.

## Learn: add the game's programs to the close list

A launcher can open a game, connector and other helpers. Learn compares the running programs before and after a
start. It cannot tell on its own whether every new program belongs to your game.

1. Close unrelated programs you do not need for the test. In Settings' advanced editor choose **Learn...**; in the
   builder choose **Learn by opening this card...**.
2. **1. Start card** notes what is already running, then uses the normal game engine to start the card. Wait until the game has reached
   the screen you want, signing in or clicking through as needed.
3. Choose **2. Find new programs**. New entries start unticked; existing close-list names and enders stay selected
   when found. Protected programs are not offered. Tick only programs that belong to the game, and keep crash
   reporters, installers, updaters and unrelated utilities out of the list.
4. **3. Apply selection and stop test** merges the selected names with the existing close list and enders, then
   uses the normal cleanup. Only after the test stops are those reviewed names passed back to the draft. If
   cleanup reports a problem, use **Stop test / retry closing** and resolve it before continuing.
5. Review the resulting rows. Learn does not decide which program should end the session or save the card for
   you. Use **Test card...** to check the finished group, then save when the result and behavior are right.

An empty result can mean the programs were already running before Learn started. It does not prove the close list
is complete. The recorded results are a snapshot: a helper that opened and exited before **Find new programs**
may not appear.

## Test card: check a full visit to this game

In the builder, use **Try this card...** to test its draft before saving. In Settings, **Test card...** asks you to
resolve any unsaved card edits first, then tests the saved card. Both use the normal launch, wait, retry,
monitoring and close engine. Running a test does not save the builder's draft, and it does not certify that a
game is connected or ready for a guest. Check the game itself and the result shown in the test window.

1. Choose **Start card test**. Expect the right programs in the right order and then the game's visible window. Check that the
   launch monitor connects and the game can reach its normal playing screen yourself.
2. Quit the main game normally. Expect its configured closing group to exit and the cards to return. Look for
   leftover connectors or launchers; add only the ones that belong to this game if anything was missed.
3. Start it again. Use the bay's back-to-games key or button and confirm **Yes, end it**. Expect the same group to
   close and the cards to return. A second start must work without using Task Manager to clear leftovers.
4. For E6, start a sport and use **Exit Game**. Expect the E6 menu to stay open. Close the E6 launcher to return to
   the cards. Repeat with the back-to-games button while a sport is running; the sport closes before its launcher.
5. If opening fails, check the program location and window wait. **Stop test / retry closing** requests normal
   cleanup; if startup is still waiting, the stop waits for normal startup, including its usual retry, to finish.
   If closing fails, read the
   problem, correct the cause and retry closing. Do not call a test successful just because its window appeared.

Read the final result: it reports that the engine returned and whether any listed program names are still
running. This check cannot find a missing helper that was never on the list. The daily log in Settings > Tools >
**Open the logs folder** gives more detail. A protected, elevated or unrelated background utility must not be
added just to make a test pass. **Help / desktop recovery** opens the local escape directions.

Closing the test window while its game is active asks what to do: **Yes** requests normal cleanup before closing,
**No** closes only the controls and leaves the game running, and **Cancel** keeps the controls open. If a stop is
already pending, it continues when you close only the controls. Closing the window does not save the card. End
the game before saving or making more card changes.

## Advanced settings and safe close lists

- **Must be closed first** closes the named programs before starting the card. Use it only for known game
  leftovers, never for Windows, launch-monitor maintenance or unrelated work.
- **When the game ends, also close any other program that opened during the game** is an optional wider cleanup
  setting. Leave it off unless you have reviewed why this particular card needs it. It can include unrelated new
  windows opened during play. It does not close programs that were already running before the card was clicked,
  and it is skipped when BayLauncher adopts a game that was already running. Recipes and Learn do not turn it on
  automatically.
- **Add from a folder...** finds program names in a folder and its subfolders. Review the results; a folder can
  contain programs that should stay open. Recognised crash reporters, updaters and setup tools are skipped.
- Settings > General controls how long programs get to close by themselves before being forced. For E6 use at
  least **30 seconds**; the E6 recipe raises a shorter setting to 30. Enders are closed after the other listed
  programs, so the E6 launcher is last. Trying or learning an unsaved E6 recipe also gives it at least 30 seconds,
  while leaving the saved global setting alone.
- Never add firmware updaters, launch-monitor maintenance/configuration utilities, crash reporters such as
  `UnityCrashHandler64`, system programs, elevated programs or unrelated background utilities to the close group.
  A game's dedicated connector such as `GSPconnect` is different: include it when it belongs to that game.
- Windows programs, command and PowerShell windows, Python, Microsoft Edge/WebView2 and protected programs are
  never closed by BayLauncher. Do not run the launcher as administrator to work around this protection.
- If a close-listed program is already open with a window when you click the card, BayLauncher may bring it
  forward as the running game. Windowless leftovers are closed before a fresh start. Keep unrelated always-on
  utilities off the list, and do not click again while **Opening ...** is showing.

---
BayLauncher owner guide, version 2026-10-27 (BayLauncher 1.0.4). © 2026 BA Custom Products LLC.
