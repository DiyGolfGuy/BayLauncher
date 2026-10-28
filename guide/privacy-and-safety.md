[BayLauncher](../README.md) > Privacy and safety

# Privacy and safety

## What BayLauncher does not do
- BayLauncher keeps its settings, card pictures and logs on this PC and has no built-in HTTP upload of those files.
  Optional companion apps and websites that you choose to open can use the network and their own accounts and privacy
  settings. BayLauncher does not inspect their page, chat, video or recording content.
- It sets no Windows policies, blocks no keys and installs no services or drivers.
- It does not alter the games' files or settings. It starts their configured programs and follows their closing
  choices; optional companion layouts can move and resize supported windows.
- Day to day, nothing runs as administrator.

## What it stores, and where
- The program: `C:\Program Files\BA Custom Products\BayLauncher`.
- Settings, card pictures and logs: `C:\ProgramData\BayLauncher`. These files have no built-in network upload.
- The optional website panel requests a private browsing session and uses its own folder for each run under
  `%LOCALAPPDATA%\BA Custom Products\BayLauncher\WebsitePanelPreview\profiles`. It never borrows or copies a personal
  Edge or Chrome profile. Local browser folders can remain after closing; this is not a secure-erasure feature.
  Use **Open in browser** only when you intend to use that normal browser's own profile and sign-in. Consider who
  uses that browser before signing into a shared bay PC.
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
Python programs, shared Microsoft Edge/WebView2 processes and programs that run as administrator stay outside the
normal game cleanup. BayLauncher can normally close its own website-panel window and release that window's browser
control; it does not force-kill every Edge or WebView2 process. Anything already running before a card was clicked
is not closed by the "also close any other program" option.

The optional website panel contacts the websites you open and their services, using those sites' own network and
privacy behavior. This is separate from the local launcher settings. A future optional Unlock would have its own
network and privacy explanation before release.

---
BayLauncher owner guide, version 2026-10-27 (BayLauncher 1.0.5). © 2026 BA Custom Products LLC.
