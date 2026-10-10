[BayLauncher](../README.md) > Troubleshooting

# Troubleshooting

**Windows will not run the setup**
- "Windows protected your PC": choose **More info** > **Run anyway** (only for the file from the official link).
- Blocked with no Run anyway: Windows 11's Smart App Control is on. Contact BA Custom Products through
  bacustomproducts.com and we will walk you through it.

**A card does not open, or shows a problem after a while**
- Open Settings > Cards and check each open step's program (**...**) and **Wait for**. A wrong Wait for makes the card
  wait until its timeout, then try once more, so "Opening ..." can show for about twice the timeout. While it shows,
  the lock button and the back-to-games button wait too; Ctrl+Alt+Del > Task Manager always works.
- Start the game once by hand to make sure it works on this PC.

**A game does not close at the end**
- Its program is missing from the close list. Use **Learn...** again, or add the name by hand.
- The program runs as administrator. Turn that off in the program's Properties > Compatibility.

**Clicking a card only brings back an old window**
- A program from its close list is still open with a window from before, so BayLauncher treats it as the running
  game. Close it (or close it in Task Manager), and take helpers that stay open (utilities, connectors you do not
  need) off the close list.

**The back-to-games button does nothing**
- It only works while a game from a card is running. Check the combo in Settings > General (**Change...** and press
  the button again).

**The bay starts to a black screen**
- Use Ctrl+Alt+Del > Task Manager > Run new task > `explorer.exe`, then see
  [Getting back to the Windows desktop](back-to-the-desktop.md).

**Forgot the staff PIN**
- Get to the desktop with Ctrl+Alt+Del > Task Manager > Run new task > `explorer.exe`, then Start > BayLauncher >
  **Reset the staff PIN**.

**Where are the logs?**
- Settings > Tools > **Open the logs folder** (`C:\ProgramData\BayLauncher\logs`). One file per day, kept 30 days. They
  record what BayLauncher did, never the PIN.

---
BayLauncher owner guide, version 2026-10-07 (BayLauncher 1.0.2). © 2026 BA Custom Products LLC.
