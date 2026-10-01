[BayLauncher](../README.md) > Privacy and safety

# Privacy and safety

## What BayLauncher does not do
- It does not connect to the internet. It sends nothing anywhere and collects no personal data.
- It sets no Windows policies, blocks no keys and installs no services or drivers.
- It does not change the games or programs it starts. It starts them, and closes them when the game ends.
- Day to day, nothing runs as administrator.

## What it stores, and where
- The program: `C:\Program Files\BA Custom Products\BayLauncher`.
- Settings, card pictures and logs: `C:\ProgramData\BayLauncher`. Nothing leaves the PC.
- The staff PIN is stored only as a salted hash, never as the digits. Logs record each PIN attempt, never the digits.

## What it changes in Windows
- Only when you choose **Turn on BayLauncher for this account**: that one account's sign-in program (its "shell"
  setting) points at BayLauncher. **Restore Windows Desktop** puts it back.
- A Start menu folder, BayLauncher.
- Every account on the PC may write to `C:\ProgramData\BayLauncher` (a folder permission set when installing), so
  settings can be saved without administrator rights.

## Programs it never closes
Windows' own programs, Explorer and Task Manager are never closed. Anything that was already running before a card
was clicked is not closed by the "also close any other program" option.

If a future version ever needs the internet (for example for an optional unlock), this page will say exactly what it
sends, before that version is released.

---
BayLauncher owner guide, version 2026-10-01 (BayLauncher 1.0.0). © 2026 BA Custom Products LLC.
