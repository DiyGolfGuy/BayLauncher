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
- A Bay ID for this PC (Settings > About and the log): made from the motherboard's and the system disk's serial
  numbers with a one-way hash. The serial numbers themselves are not stored. It stays on the PC.

## What it changes in Windows
- Only when you choose **Turn on BayLauncher for this account**: that one account's sign-in program (its "shell"
  setting) points at BayLauncher, and a **Restore Windows Desktop** shortcut goes on that account's desktop.
  **Restore Windows Desktop** puts it back.
- A Start menu folder, BayLauncher, and an entry in Settings > Apps > Installed apps.
- Every account on the PC may write to `C:\ProgramData\BayLauncher` (a folder permission set when installing), so
  settings can be saved without administrator rights.

## Programs it never closes
Windows' own programs (Explorer, Task Manager and everything in the Windows folder), command and PowerShell windows,
Python programs, Microsoft Edge and WebView2, and programs that run as administrator are never closed. Anything that
was already running before a card was clicked is not closed by the "also close any other program" option.

If a future version ever needs the internet (for example for an optional unlock), this page will say exactly what it
sends, before that version is released.

---
BayLauncher owner guide, version 2026-10-07 (BayLauncher 1.0.2). © 2026 BA Custom Products LLC.
