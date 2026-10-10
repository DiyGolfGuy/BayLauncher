# BayLauncher

**Free game cards for golf-simulator bays, by BA Custom Products.**

BayLauncher replaces the Windows desktop on a bay PC with big picture cards: GSPro, TruGolf Multisport or any other
program. A guest clicks a card and the game opens. When the game is over, one button (a key combo, or a button on a
BA control box) asks "End this game?", closes everything that card opened, and brings the cards back. Staff get the
normal Windows desktop with a PIN.

## Get BayLauncher
**[Download BayLauncher (free)](https://github.com/DiyGolfGuy/BayLauncher/releases/latest/download/BayLauncher-Setup.exe)**,
always the newest version. The [Releases page](https://github.com/DiyGolfGuy/BayLauncher/releases) lists each version
with its SHA-256 checksum. Then see [Installing](guide/installing.md) and [First-time setup](guide/first-time-setup.md).

## How to get out (keep this handy)
BayLauncher never locks you out. Any of these gets you back to the normal Windows desktop:
1. **Staff PIN:** press the lock button in the top-right corner of the cards, enter your PIN, choose **Desktop**.
   After 10 minutes without anyone using the PC, a one-minute countdown shows, then the cards come back by themselves.
2. **Ctrl+Alt+Del:** press the three keys together, choose **Task Manager** > **Run new task**, type `explorer.exe`,
   press **OK**. The full desktop and taskbar appear.
3. **Restore Windows Desktop:** after 1 or 2, use the shortcut on the desktop (or Start > BayLauncher > Restore Windows
   Desktop). From the next sign-in this account starts to the normal desktop.
4. **SAFE.txt:** make an empty file called `SAFE.txt` in `C:\ProgramData\BayLauncher`, then sign out and back in.
   Delete the file, then sign out and back in, to go back to the cards.

To stop BayLauncher for good on an account: number 3. Details: [Getting back to the Windows desktop](guide/back-to-the-desktop.md).

## What it does
- Full-screen picture cards in place of the desktop, on the screen you choose. Your own card pictures.
- A card can run several programs in order (for example ProTee AutoStart, which then opens GSPro) and waits for the
  game window.
- **Learn** watches while you start a game and lists every program that opened, so closing is done right.
- **End this game?** from a key combo or a control-box button; everything the card opened closes and the cards come
  back. Closing the game itself does the same.
- Side screens show a background picture.
- A staff PIN behind the lock button opens Settings or the normal Windows desktop. The cards come back by themselves
  after 10 minutes without anyone using the desktop (and a one-minute countdown), and nothing you left open is closed.
- Settings and pictures can be exported and imported to set up the next bay.
- Help inside the program: **? Help** (or F1) in Settings opens this guide at the chapter for that tab. Settings >
  **About** shows the version, the edition and the PC's Bay ID.

## Free
BayLauncher is free, with every feature. The free edition shows the BA Custom Products background on every screen
(it advertises BA Custom Products and has a QR code to bacustomproducts.com) and a small BA Custom Products mark in
a corner of the cards screen. An optional one-time unlock per PC, for your own backgrounds and sponsor pictures, is
planned for later. It is not available yet.

## Safe by design
- It blocks no keys and sets no Windows policies. When BayLauncher is not running, the PC is a normal PC.
- There are always four ways back to the normal desktop: see [Getting back to the Windows desktop](guide/back-to-the-desktop.md).
- It does not connect to the internet and collects no personal data: see [Privacy and safety](guide/privacy-and-safety.md).
- After installing, nothing runs as administrator.

## Guide
- [Installing](guide/installing.md)
- [First-time setup](guide/first-time-setup.md)
- [Cards and Learn](guide/cards-and-learn.md)
- [Recipe: GSPro with ProTee AutoStart](guide/recipe-gspro-protee-autostart.md)
- [Recipe: TruGolf Multisport](guide/recipe-trugolf-multisport.md)
- [The back-to-games button](guide/back-to-games-button.md)
- [Screens and the look](guide/screens-and-look.md)
- [Turning BayLauncher on and off for an account](guide/turn-on-and-off.md)
- [Getting back to the Windows desktop](guide/back-to-the-desktop.md)
- [Moving your settings to another bay](guide/export-import.md)
- [Troubleshooting](guide/troubleshooting.md)
- [Privacy and safety](guide/privacy-and-safety.md)
- [Updating](guide/updating.md)
- [Uninstalling](guide/uninstalling.md)

## What you need
- A Windows 11 PC, 64-bit (what BayLauncher is tested on). Windows 10 64-bit may work but is not tested.
- The games already installed and working on that PC.
- An administrator account to install it. Day to day, nothing runs as administrator.

## Contact
BA Custom Products: [bacustomproducts.com](https://www.bacustomproducts.com/)

## Legal
BayLauncher is free to use. It is proprietary software, © 2026 BA Custom Products LLC, all rights reserved. The
license agreement comes with the setup. This page holds documents only; the program's source code is not published.

GSPro, TruGolf, E6, ProTee and ProTee Labs are trademarks of their owners. BayLauncher is not affiliated with,
endorsed by or sponsored by them. It only starts and closes the programs you set up; it does not change them.

---
BayLauncher owner guide, version 2026-10-07 (BayLauncher 1.0.2). © 2026 BA Custom Products LLC.
