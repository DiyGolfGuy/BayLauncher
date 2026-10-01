[BayLauncher](../README.md) > Troubleshooting

# Troubleshooting

**A card does not open, or shows a problem after a while**
- Open Settings > Cards and check each open step's program (**...**) and **Wait for**. A wrong Wait for makes the card
  wait until its timeout.
- Start the game once by hand to make sure it works on this PC.

**A game does not close at the end**
- Its program is missing from the close list. Use **Learn...** again, or add the name by hand.
- The program runs as administrator. Turn that off in the program's Properties > Compatibility.

**A card does nothing because "the game is already open"**
- A program from its close list is still running from before. Close it in Task Manager, and take helpers that stay
  running (crash reporters, utilities) off the close list.

**The back-to-games button does nothing**
- It only works while a game from a card is running. Check the combo in Settings > General (**Change...** and press
  the button again).

**The bay starts to a black screen**
- Use Ctrl+Alt+Del > Task Manager > Run new task > `explorer.exe`, then see
  [Getting back to the Windows desktop](back-to-the-desktop.md).

**Where are the logs?**
- Settings > Tools > **Open the logs folder** (`C:\ProgramData\BayLauncher\logs`). One file per day, kept 30 days. They
  record what BayLauncher did, never the PIN.

---
BayLauncher owner guide, version 2026-09-30 (for BayLauncher 1.0.0, in preparation). © 2026 BA Custom Products LLC.
