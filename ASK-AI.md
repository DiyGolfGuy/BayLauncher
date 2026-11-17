# BayLauncher: the guide for AI assistants (and the people asking them)

This one file holds everything about BayLauncher, the free game-card launcher for golf-simulator PCs by BA Custom
Products: instructions for an AI assistant, short answers to common questions, and the complete owner guide.
It is made from the owner guide, version 2026-11-16 (BayLauncher 1.0.8).

## For people: how to ask an AI about BayLauncher

Copy the three lines below into ChatGPT, Claude or another AI assistant, put your question at the end, and send it:

```
Please read https://raw.githubusercontent.com/DiyGolfGuy/BayLauncher/main/ASK-AI.md first.
It is the complete official guide to BayLauncher, written for AI assistants. Follow its instructions.
Then help me with BayLauncher, step by step. My question:
```

If your assistant says it cannot open links: open the link yourself, select everything on the page, copy it, and
paste it into the chat before your question.

Good questions to ask:

- "I have a Uneekor launch monitor and GSPro. How do I make one card that starts both?"
- "My game opens on a menu. How do I make BayLauncher click through to the range?"
- "I made two cards and can only open one. What did I do wrong?"
- "A click comes too early. How do I give the game more time?"
- "How do I get back to the normal Windows desktop?"
- "What does BayLauncher change on my PC, and how do I remove it?"

An AI can be wrong. If it names a button you cannot find, trust the program and the guide below, and tell the AI
what you actually see on the screen. For anything it cannot answer, contact BA Custom Products through
https://www.bacustomproducts.com/.

## For the AI assistant: how to help

You are helping the owner or staff of a golf-simulator bay (a home bay or a facility) set up and use BayLauncher on
a Windows 11 PC. Many of them are not computer people. Follow these rules.

**Stay with this document.**
- Everything you say about BayLauncher must come from this file. If the answer is not here, say that the guide does
  not cover it and point to BA Custom Products (https://www.bacustomproducts.com/). Do not guess.
- Use the exact names of buttons, pages and settings as written in the guide (they are in bold there). Do not
  invent buttons, menus, settings, file names, command-line switches or version numbers.
- The guide describes the version in its first lines. If the person's program looks different, ask which version
  they have (Settings > About) and suggest updating: the newest setup is always at
  https://github.com/DiyGolfGuy/BayLauncher/releases/latest/download/BayLauncher-Setup.exe.

**How to answer.**
- Give numbered steps, one action per step, in the order the person will do them. Say where each step happens
  (for example: Settings > Cards > Add card).
- Before long instructions, find out what you need: which launch monitor software and which game they use, whether
  the PC starts straight into the cards or BayLauncher runs in a window, and what they see on the screen now.
- Keep it short and plain. No registry edits, no PowerShell, no Task Manager tricks beyond the ones in the guide.
- If someone is locked out or sees a black screen, give the ways back to the desktop first ("How to get out" in the
  guide), before anything else.

**The ideas people most often get wrong. Explain them correctly.**
- **One card is one whole game.** A card holds every program the game needs: the launch monitor's own software,
  any connector, and the game. BayLauncher opens them in order and closes them together. Only one card runs at a
  time. Someone who made a card for the launch monitor and another for the game should put both programs on one
  card (Settings > Cards > **Combine...**).
- **Watch me start it** is the easiest way to make a card, for any launch monitor and any game: the person starts
  everything by hand once and BayLauncher records the programs and the clicks. Recommend it first.
- **Start-up clicks** let a card click through a game's menus to the screen guests should start on. They are
  recorded with Watch me start it, not placed by hand. While recording, BayLauncher reads the words of each clicked
  screen with the text reader built into Windows; when the card starts, each click waits until those words show
  (however long the game takes that day), moves the mouse, lets it settle, then clicks. Cards recorded at one
  resolution work at another. Waits can be changed on the page **Clicks to get in**.
- **When one program of a card closes, the whole card closes** and the cards come back. That is on purpose.
- **If a click cannot be made, the programs stay open** and the person carries on with the mouse. The log says
  what BayLauncher read instead and keeps a picture of the screen in the logs folder. After a game update changed
  a screen, the fix is **Teach this click again...** on that click (or watching the start again); a notice that
  only comes now and then goes under **Notices to click away**.

**What BayLauncher is not.**
- It starts and closes programs. It does not connect a launch monitor, set up a game, or fix a game's licence or
  account. For those, send the person to that product's own support.
- The guide has ready-made recipes only for GSPro with ProTee AutoStart and for TruGolf Multisport. For every other
  launch monitor and game, do not guess program names or folders: use Watch me start it, which finds them.
- BayLauncher was checked with test programs, not with every launch monitor and game. Always tell the person to
  use **Try this card** before guests use a new card.
- It is guidance for guests, not a security lock. Do not present it as one.
- The Free edition shows the BA Custom Products background. A paid Unlock is not available yet.

**When something goes wrong.**
- Use the Troubleshooting chapter first.
- Ask what the screen shows and what happened just before. The log helps: Settings > Tools > **Open the logs
  folder**. The newest file there says what BayLauncher did, line by line.
- Programs that run as administrator cannot be started, clicked or closed by BayLauncher. The guide says how to
  turn that off in the program's Properties.

## Short answers to common questions

**What is BayLauncher?** A free program for a golf-simulator PC. Instead of the Windows desktop, guests see big
picture cards. Tapping a card starts everything that game needs; one button ends the game and brings the cards back.
Staff get the normal desktop with a PIN.

**I made a card for my launch monitor software and a card for my game, and I cannot open both.** Only one card runs
at a time, so both programs belong on one card. Settings > Cards, select the card that should open first, choose
**Combine...**, pick the other card, check the result and choose **Save card**.

**How do I add a program when I do not know where it is installed?** Settings > Cards > **Add card**, then on the
page **Programs to open** choose **Watch me start it...** and start your game by hand once. Or choose **Pick a
program...** and select it from the list of your shortcuts, from the programs open right now, or paste a path.

**My game opens on a menu. Can the card click through it?** Yes. Use **Watch me start it...** and click through to
the screen guests should start on, then press **Ready**. The clicks appear on the page **Clicks to get in**, each
with a picture. **Try this card...** on the last page shows them being made.

**A click comes too early, or the game needs more time.** A click set to **Then click as soon as the screen's words
show** already waits for the game, however long it takes. For a click that goes by time, make **Wait before this
click** longer on **Clicks to get in**. The settle time at the top of that page (one second to start) can be made
longer too.

**The clicks worked and now they stop.** Usually the game was updated and a screen changed, or a new notice comes
up. The log line names a picture of what BayLauncher saw (`click-not-made-...jpg` in the logs folder). Open the card
with **Edit with guide...**, go to **Clicks to get in** and use **Teach this click again...** on that click, or type
the notice's button words under **Notices to click away**.

**How does a game end?** With the back-to-games button (a key combination or a BA control box button), or when a
guest closes one of the card's programs. BayLauncher then closes everything on the card and shows the cards.

**How do I get to the Windows desktop?** Press the lock button in the top-right corner of the cards, enter the
staff PIN and choose **Desktop**. Or Ctrl+Alt+Del > Task Manager > Run new task > `explorer.exe`. The chapter
"Getting back to the Windows desktop" has every way.

**I forgot the staff PIN.** Get to the desktop with Ctrl+Alt+Del > Task Manager > Run new task > `explorer.exe`,
then Start > BayLauncher > **Reset the staff PIN**.

**Does it work with my launch monitor or my game?** BayLauncher does not talk to a launch monitor. It starts and
closes Windows programs, so anything you can start by hand can go on a card. It has not been tested with every
product: make the card, then use **Try this card**.

**Is it free? What is the catch?** The Free edition is free and shows the BA Custom Products background on every
screen. A paid Unlock for your own backgrounds is planned and not available yet.

**What does it change on my PC?** See the chapter "Privacy and safety". In short: it installs into Program Files,
keeps its settings in `C:\ProgramData\BayLauncher`, and only when you choose "Turn on BayLauncher for this account"
does that one Windows account start into the cards. "Restore Windows Desktop" undoes that.

**How do I update or remove it?** Updating: run the newer setup; cards, pictures and PIN are kept. Removing:
Settings > Apps > Installed apps > BayLauncher > Uninstall. See the chapters "Updating" and "Uninstalling".

**How do I set up a second bay the same way?** Settings > Tools > **Export settings and pictures...** on the first
bay, **Import settings and pictures...** on the second. Check each card's programs afterwards.

---

# The complete BayLauncher owner guide

Version 2026-11-16 (BayLauncher 1.0.8). 16 chapters follow, in the order of the printed guide.

## Chapter: BayLauncher

**Free game cards for golf-simulator bays, by BA Custom Products.**

> **Version 1.0.7:** making a card no longer needs a folder or a path. **Watch me start it** lets you start your
> game by hand once while BayLauncher fills in the card, with every program the game needs and the clicks to get to
> the right screen. You can also pick programs from a list, and **Combine...** puts two single-program cards
> together. One card is one whole game: the launch monitor's software and the game go on the same card.
> These were checked on a Windows 11 PC with test programs, not with every launch monitor and game: after you make
> a card, use **Try this card** on your own bay. The separate customer paid Unlock version, 1.1.0, remains unreleased.

BayLauncher replaces the Windows desktop on a bay PC with big picture cards: GSPro, TruGolf Multisport or any other
program. A guest clicks a card and the game opens. When the game is over, one button (a key combo, or a button on a
BA control box) asks "End this game?", closes the card's selected game group, follows its extra-app closing choices, and brings the
cards back. Staff get the
normal Windows desktop with a PIN.

### Get BayLauncher
**[Download BayLauncher (free)](https://github.com/DiyGolfGuy/BayLauncher/releases/latest/download/BayLauncher-Setup.exe)**,
always the newest version. The [Releases page](https://github.com/DiyGolfGuy/BayLauncher/releases) lists each version
with its SHA-256 checksum. Then see [Installing](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/installing.md) and [First-time setup](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/first-time-setup.md).

### How to get out (keep this handy)
BayLauncher never locks you out. Any of these gets you back to the normal Windows desktop:
1. **Staff PIN:** press the lock button in the top-right corner of the cards, enter your PIN, choose **Desktop**.
   After 10 minutes without anyone using the PC, a one-minute countdown shows, then the cards come back by themselves.
2. **Ctrl+Alt+Del:** press the three keys together, choose **Task Manager** > **Run new task**, type `explorer.exe`,
   press **OK**. The full desktop and taskbar appear.
3. **Restore Windows Desktop:** after 1 or 2, use the shortcut on the desktop (or Start > BayLauncher > Restore Windows
   Desktop). From the next sign-in this account starts to the normal desktop.
4. **SAFE.txt:** make an empty file called `SAFE.txt` in `C:\ProgramData\BayLauncher`, then sign out and back in.
   Delete the file, then sign out and back in, to go back to the cards.

To stop BayLauncher for good on an account: number 3. Details: [Getting back to the Windows desktop](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/back-to-the-desktop.md).

### What it does
- Full-screen picture cards in place of the desktop, on the screen you choose. Your own card pictures.
- One card is one whole game: it opens every program the game needs, in order (the launch monitor's software, a
  connector, the game), waits for their windows, and closes them together.
- **Watch me start it:** start your game by hand once and BayLauncher fills in the card. No folders or paths.
- **Start-up clicks:** a card can click through a game's menu or notices to the screen guests should start on. Each
  click waits until the game has really got to its screen (BayLauncher reads the screen's words with the text reader
  built into Windows), then moves the mouse there, lets it settle and clicks. A slow start is simply waited for.
- A guided card builder takes you through a name and picture, what opens, the clicks, what closes, and a summary
  to try. Programs can be picked from a list of your shortcuts or of what is open right now.
- **Learn** lists new programs for you to review and add to a card's close list.
- **Test card...** uses the same launch and close engine as the cards screen. You check the game and its helpers on
  this PC; seeing a window does not prove the launch monitor is connected or the game is ready to play.
- **End this game?** from a key combo or a control-box button closes the selected game group and follows the extra-app
  closing choices, then brings the cards back. Closing a configured game ender does the same.
- Optional extra apps can open with a card. Compatible newly started app windows can use saved screen, size and
  position. A built-in **Website panel (Preview)** can open a website in its own movable, resizable window.
- Help has offline topic search and task shortcuts; optional larger steps explain extra apps and their layouts.
- Side screens show a background picture.
- A staff PIN behind the lock button opens Settings or the normal Windows desktop. The cards come back by themselves
  after 10 minutes without anyone using the desktop (and a one-minute countdown), and nothing you left open is closed.
- Settings and pictures can be exported and imported to set up the next bay.
- Help inside the program: **? Help** (or F1) in Settings opens this guide at the chapter for that tab. Settings >
  **About** shows the version, the edition and the PC's Bay ID.

### Free
BayLauncher is free, with every feature. Choose a built-in background in Settings > **Look**: Classic BA Custom
Products, Midnight simulator, Golden-hour links, Mountain valley, Green contours, Night range, Dusk hills, Ball
close-up, Yardage book or Fairway stripes. Your choice appears behind the cards and on the
side screens. Classic keeps its original BA artwork and readable QR code; the other choices retain a small BA logo,
BA Custom Products name and bacustomproducts.com advertising panel. An optional one-time unlock per PC, for your own
backgrounds and sponsor pictures, is planned for later. It is not available yet.

### Safe by design
- It blocks no keys and sets no Windows policies. When BayLauncher is not running, the PC is a normal PC.
- There are always four ways back to the normal desktop: see [Getting back to the Windows desktop](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/back-to-the-desktop.md).
- It has no built-in upload of your settings, pictures or logs. Optional apps and websites can use the network:
  see [Privacy and safety](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/privacy-and-safety.md).
- After installing, nothing runs as administrator.

### Guide
- [Installing](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/installing.md)
- [First-time setup](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/first-time-setup.md)
- [Cards and Learn](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/cards-and-learn.md)
- [Recipe: GSPro with ProTee AutoStart](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/recipe-gspro-protee-autostart.md)
- [Recipe: TruGolf Multisport](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/recipe-trugolf-multisport.md)
- [The back-to-games button](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/back-to-games-button.md)
- [Screens and the look](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/screens-and-look.md)
- [Turning BayLauncher on and off for an account](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/turn-on-and-off.md)
- [Getting back to the Windows desktop](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/back-to-the-desktop.md)
- [Moving your settings to another bay](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/export-import.md)
- [Troubleshooting](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/troubleshooting.md)
- [Privacy and safety](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/privacy-and-safety.md)
- [Updating](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/updating.md)
- [Uninstalling](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/uninstalling.md)

### What you need
- A Windows 11 PC, 64-bit. Try each new card, window, website and game combination on that PC before guests use it.
  Windows 10 64-bit may work but is not tested.
- The optional website panel needs Microsoft WebView2 Runtime and internet access for its websites. The runtime is
  normally included with Windows 11; if it is unavailable, the panel explains that and offers the normal browser.
- The games already installed and working on that PC.
- An administrator account to install it. Day to day, nothing runs as administrator.

### Ask an AI
Would you rather ask than read? Copy these lines into ChatGPT, Claude or another AI assistant, add your question
at the end, and send it. The link is one file with this whole guide, written so an assistant can answer questions
such as "how do I make one card for my launch monitor and my game?" or "how do I get back to the desktop?".

```
Please read https://raw.githubusercontent.com/DiyGolfGuy/BayLauncher/main/ASK-AI.md first.
It is the complete official guide to BayLauncher, written for AI assistants. Follow its instructions.
Then help me with BayLauncher, step by step. My question:
```

If the assistant cannot open links, open the link yourself, copy everything on the page and paste it into the
chat. An AI can be wrong: if it names a button you cannot find, trust the program and this guide.

### Contact
BA Custom Products: [bacustomproducts.com](https://www.bacustomproducts.com/)

### Legal
BayLauncher is free to use. It is proprietary software, © 2026 BA Custom Products LLC, all rights reserved. The
license agreement comes with the setup. This page holds documents only; the program's source code is not published.

GSPro, TruGolf, E6, ProTee and ProTee Labs are trademarks of their owners. BayLauncher is not affiliated with,
endorsed by or sponsored by them. It only starts and closes the programs you set up; it does not change them.

---

## Chapter: Installing

1. Download the setup only from the link on bacustomproducts.com or the BayLauncher page on GitHub. The download
   link gives `BayLauncher-Setup.exe`; the Releases page also lists it as `BayLauncher-Setup-<version>.exe` (the same
   file). The page lists the file's SHA-256 checksum, so anyone who wants to can check the file is the one BA Custom
   Products published.
2. Run it. The setup is not digitally signed yet, so Windows may say "Windows protected your PC". Choose
   **More info** > **Run anyway**, only for the file from the official link. On Windows 11 with Smart App Control
   turned on, Windows may block the setup completely: contact BA Custom Products through bacustomproducts.com and we
   will walk you through it.
3. Approve the Windows prompt. Installing needs an administrator account; day to day, nothing runs as administrator.
4. The setup explains what BayLauncher does, shows the ways back to the desktop, asks you to accept the license
   agreement, and asks where to install (keep the folder it suggests).
5. On the last page, leave "Open the 'Back to the desktop' sheet to print" ticked, print the sheet, and keep it next
   to the bay PC.

### What installing changes
- The program goes in `C:\Program Files\BA Custom Products\BayLauncher`, with a Start menu folder named BayLauncher
  and an entry in Settings > Apps > Installed apps.
- Nothing starts by itself and no Windows account is changed. The cards only take over an account after you choose
  **Turn on BayLauncher for this account** (see [Turning BayLauncher on and off for an account](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/turn-on-and-off.md)).

### If the setup warns you
The setup checks the PC first. It stops on 32-bit Windows, and it warns (you can still choose to install) on an ARM
PC, Windows Server, Windows older than Windows 10 version 22H2, a main screen smaller than 1280 x 720, or an account
that already starts another kiosk or launcher program instead of the desktop.

---

## Chapter: First-time setup

The first time BayLauncher starts, a short setup opens over the cards. It cannot be closed until a staff PIN is
chosen, so no guest can set one.

1. **Welcome:** what BayLauncher does.
2. **How to get back to the desktop:** the four ways. Print them: Start > BayLauncher > How to get back to the desktop.
3. **Your staff PIN:** type it on the number pad (or the keyboard), press **OK**, type it again, **OK**. 4 to 8 digits.
   PINs like 0000 or 1234 are refused, because guests guess those first.
4. **Which screen shows the cards:** choose the projector or main TV. "Show each screen's number" helps.
5. **The button that ends a game:** press **Change...**, then the keys together or your control box button.
6. **Your first game card:** a recipe fills the card in. **GSPro with ProTee AutoStart**, **TruGolf Multisport** (it
   finds the sports in the launcher's Products folder and TruGolf's separately installed E6 games, and sets the time
   programs get to close to at least 30 seconds for all cards), **Another program**, or **Skip**.
   The first choice is **Watch me start my game**: when the setup is finished, the card builder opens, and
   **Watch me start it** fills in the card while you start your game by hand once.
7. **Start the bay into the cards:** how to turn it on for the bay's Windows account.
8. **All set.**

Run it again any time: Settings > Tools > **Run the first-time setup again**.

The optional help buttons explain the steps without changing your PIN, card or Windows account. When setup is
finished, start with a simple working card; use Settings > Cards to add pictures, test it or duplicate it with
optional extra apps and a different layout.

---

## Chapter: Updating

Run the newer setup on the bay PC. It closes BayLauncher if it is running (in every Windows account that is signed
in, so sign out any other account that uses the cards first), replaces the program, and keeps your cards, pictures,
look, screens and staff PIN (they live in `C:\ProgramData\BayLauncher`). Then sign out and back in, or start
Start > BayLauncher > BayLauncher in a window (setup and testing) to check it.

---

## Chapter: Uninstalling

1. Settings > Apps > Installed apps > BayLauncher > **Uninstall** (or Start > BayLauncher > **Uninstall BayLauncher**).
2. Approve the Windows prompt.
3. BayLauncher closes (in every signed-in account), and the program and its Start menu folder are removed. The
   Windows account you uninstall from starts to the normal desktop again. Any other account that started into the
   cards gets the normal desktop at its next sign-in, but its setting still points at BayLauncher, so a later
   reinstall would turn the cards back on there. To avoid that, sign in to each such account first and use
   **Restore Windows Desktop**, then uninstall.
4. The uninstaller asks whether to delete your settings, card pictures and logs. Choose **No** to keep them for a
   later reinstall.

---

## Chapter: Cards and Learn

**One card is one whole game.** A card holds everything that has to be open for guests to play: your launch
monitor's own software, any connector, and the game itself. BayLauncher opens them in order, and when the game ends
it closes them together and brings the cards back. Only one card runs at a time. If golf on your bay needs the
launch monitor's software and a golf game, both go on the same card, called for example **Play Golf**. Do not make
one card for the launch monitor and another for the game: the second cannot open while the first is running.

Settings > **Cards** lists the cards in the order they appear. A plain **Play Golf** card and a separate
**Golf + Video** card can keep different companion apps and layouts.

### Open Settings
Click the lock button in the top-right corner of the cards screen, enter the staff PIN, and choose **Settings**.

**? Help** opens **Help & ideas**. Browse a chapter, choose a task such as **Arrange windows**, or search for words
such as OBS, picture-in-picture, closing or desktop. Search works offline and shows the matching guide section.
**Ctrl+F** selects search; **Clear** returns to all chapters. On a narrow window, a topic picker replaces the chapter
list so the reading area stays useful.

### Before changing a working bay

End the running game first. Settings > Tools > **Export settings and pictures...** makes a portable copy of the
current setup. Keep it somewhere safe before making several changes. Adding or editing a card needs no internet.

### Make a card, one step at a time

Choose **Add card** to open the guided builder. **Next** moves through its pages, **Back** lets you change an
earlier answer, and **Cancel** leaves the saved cards alone. **Help with this step** or F1 opens the current step's
help. **Open the full card help** opens this chapter. Both work without an internet connection.

#### Name and picture

Give the card a name guests will recognise. Choose a picture, or leave it empty to show the card's name.
**Show the whole picture** keeps text and QR codes visible; **Fill the card (crop the edges)** may crop them. The preview helps you
check the choice. These are draft changes until **Save card** succeeds.

#### Programs to open

Everything this game needs goes on this one card: the launch monitor's software, any connector and the game. Two
cards cannot run at the same time.

**Easiest: Watch me start it.** Choose **Watch me start it...** and start the game by hand once, the way you do
today. BayLauncher's windows step aside and your Windows desktop shows. On a bay that starts into the cards, the
desktop and taskbar are started for you; they stay open behind the cards until the next sign-out, as after
**Desktop**. A small bar says **BayLauncher is watching**.

1. First close your golf programs if any are open, so they can be seen starting.
2. Start every program the game needs, in your usual order, and click through until guests could start playing.
3. Press **Ready** on the bar. If a full-screen game hides the bar, press your back-to-games button instead.

BayLauncher then fills in the card: the programs you started, with their real locations and start-up options; the
programs still running at the end, as the closing group; and your clicks. Check each page before saving. Only
programs that start and left mouse clicks inside them are noted. The keyboard is not read, and clicks on the
desktop or in programs that were already open are not kept. **Cancel** on the bar keeps nothing.

What it cannot see: a program that was already open is not seen starting, so close it and watch again. A program
that runs as administrator cannot be started, clicked or closed by BayLauncher; turn that off in the program's
Properties > Compatibility. Anything Windows started by itself in the meantime is offered unticked on the closing
page.

**Or pick the programs yourself.** Choose **Pick a program...** (later **+ Add another program...**). A list opens
with three ways to find a program without knowing where it is installed:

- **Programs on this PC:** every program with a shortcut on the desktop or in the Start menu, with its icon.
  **Search** narrows the list.
- **Open right now:** start the program the way you normally do, then pick it here by its window title.
- **Not in the list?** **Browse for it...**, paste a path (in File Explorer: right-click the program, **Copy as
  path**), or drag a program or shortcut onto the window.

A shortcut is read for you: the card gets the real program file and the options the shortcut starts it with, so a
desktop shortcut works here. Windows' own programs and uninstallers are left out of the list.

Add one program for each thing you start yourself today, in the order you start them, and put them in order with
the **▲** and **▼** arrows. Do not add what a program starts by itself (a connector, the game behind a launcher):
that is found for you on the closing page.

**Ready-made setups** (folded away at the bottom of the page) fill in one known combination: **GSPro with ProTee
AutoStart**, **TruGolf Multisport / E6 Product Launcher** or **Other program**, then **Use this setup...** and browse
to that program on this PC. Setups are starting points: check the program file and the closing programs they
suggest. A setup cannot know which helpers your particular bay needs. When editing a working card, keep its
current programs unless you mean to replace the draft's programs and closing choices with a new setup.

Each program has **More options: file, start-up options and waiting**. **Start-up options (optional)** are extra
instructions for the program, such as AutoStart's `/run`; leave them empty unless the program needs them.
The advanced editor (Settings > Cards > **Advanced launch and close settings**) also takes scripts.

Tick **Wait until this program shows a window before going on**, then enter **Program name, or words in its
window title** and **Wait at most (seconds)**. These are called **Wait for** and **Timeout (s)** in the advanced
editor. The wait means a new visible window from a program that was not running when the card started. Use its
program name without `.exe`, or words in its window title. It does not check a launch-monitor connection,
sign-in, course loading or readiness to play. Untick the wait only when the next program can start immediately.
If a program is only a small starter for the real game, wait for the real game's window instead. On a start-up
failure, BayLauncher cleans up and tries once more; a wrong wait can therefore take about twice the time before
showing a problem.

#### Clicks to get in

**Why you would want them.** Many games do not open ready to play. They open on a menu, an update notice, a
"choose your course" screen or a sign-in, and somebody has to find the mouse and click through it before anyone
can hit a ball. With start-up clicks the card does that itself, the same way every time: a guest taps **Play Golf**
and ends up on the range, and staff do not have to walk over. A card without clicks is normal for a game that
opens ready to play.

**How to build them.** You do not place clicks by hand. You show them once:

1. On the page before, choose **Watch me start it...**.
2. Start the game the way you always do, and click through to the screen guests should start on. Click at your
   normal pace: BayLauncher notes where each click lands, and reads the words on the screen you clicked on (the
   button's words, such as PRACTICE RANGE, and a few other words of that screen).
3. Press **Ready**. This page then lists every click you made inside the game's programs, each with a small
   picture of the spot, a red ring where you clicked and the words it will wait for.
4. On the last page choose **Try this card...** and watch BayLauncher make the clicks itself.

Clicks on the desktop, and clicks in programs that were already open, are not kept. To redo or add a single click
later, use **Teach this click again...** or **Add a click...** (below).

**What BayLauncher does for each click, when the card starts:**

- It **waits until the game has got to that click's screen**. For a click set to **Then click as soon as the
  screen's words show**, BayLauncher reads the program's window with the text reader built into Windows (the same
  one BA's ProTee AutoStart and BA Remapper use) until it finds the button's words and at least half of the other
  words of that screen. Words that change, like a player's name, may be missing. Whether the game takes 3 seconds
  or 30 on a given day, the click comes when the screen is there, and nobody has to guess the seconds.
- A click set to **Then click once the screen looks like this picture** waits until the spot looks like its
  picture instead; that is used where there are no words to read.
- Before that, it waits the short time shown for that click (**Wait before this click**), counted from the click
  before it (for the first click: from the moment its program's window showed). For a click that waits for words
  this starts at one second; for the others it is the time you took when recording.
- It **moves the mouse to the spot and lets it settle** there (one second), checks once more that nothing
  changed, and clicks. A button that has only just appeared does not always take a click at once.
- It clicks only inside the program the click was recorded in. If another window is over the spot, it asks the game
  to come to the front and waits. If someone moves the mouse, it waits and tries again. It does not block the
  mouse or the keyboard. The mouse glides to the spot and the button is held down briefly, the way a hand clicks.
- If the game is already past a click's screen (some games remember where they were, or skip a screen after an
  update), BayLauncher sees the next click's screen instead, skips the click that is not needed today and carries on.
- Guests see a strip asking them to leave the mouse alone. **Esc** stops the clicks.

**Changing the timing.** Everything about the timing is yours to change on this page:

- **Wait before this click:** the seconds before each click. Make it longer when the game needs more time between
  two clicks (a slow menu, a connection that takes a while), or shorter when you clicked slowly while recording.
- **For every click: move the mouse to the spot, let it settle for ... seconds, then click** (top of the page):
  one second to start; make it longer on a slower PC.
- **Then click as soon as the screen's words show (recommended)**, **Then click once the screen looks like this
  picture**, or **Then click, without checking the screen**. Without a check the click goes by its wait alone, as
  a timed click. BayLauncher chooses that by itself only where there are no words to read and the spot is one plain
  colour or keeps moving, and adds spare time.
- **Give up after:** how many more seconds a click holds out for its window and its screen. For a click that waits
  for words this starts at a minute and a half or more, so a slow day or a slow update fits in.

**Teach this click again...** redoes one click: get the game to that click's screen, click the spot once and press
**Use this click** on the small bar. The click keeps its place in the list and its times, and takes the new spot and
the new screen's words. **Add a click...** does the same for a new click at the end. **Remove this click** takes one
out.

**Notices to click away.** Some programs now and then show a notice before their usual screen: an update prompt, a
sign-in reminder, a "what's new" box. Those cannot be recorded in order, because they do not come every time. Type
the words on the button that closes the notice, one per line (for example **Download Update** or **Skip**). While
this card's clicks wait, BayLauncher clicks those words whenever one of the card's programs shows them, then goes
on waiting for the next click's screen. Windows' own "Do you want to allow changes?" prompts cannot be clicked by
any program.

**When a click cannot be made.** The clicks stop there and the programs stay open, so guests or staff carry on
with the mouse. The strip says so, and the log says which click, why, what words BayLauncher read on the screen
instead, and where it kept a picture of what it saw (`click-not-made-...jpg` in the logs folder). In practice this
happens after a game update changed a screen or added a notice: look at the picture, then use **Teach this click
again...** on that click, or add the notice's button words under **Notices to click away**.

**What a click remembers, and its limits.** A click is a place inside its program's window, not a place on the
screen, so it follows the window to another position, another screen or another window size. The words and the
picture it checks follow the window's size too, so a card recorded at one resolution also works at another. If a
button's words have moved (another shape of screen), the click moves with them. Left clicks only, no typing. A
program that runs as administrator cannot be clicked. Reading words needs a text-reading language in Windows (an
English Windows has one); without it, clicks check the picture instead and the log says so once. Always use **Try
this card** after recording.

#### Programs to close

When the game ends, BayLauncher closes every ticked program, so the next guest starts fresh. Tick every program
that belongs to this game under **Closes with the card**. If a guest closes any ticked program that has a window,
the game ends: BayLauncher closes the rest and the cards come back. That way nobody can close a connector and
carry on with half a game.

After **Watch me start it**, the list is already filled with what was still running, each with a few words about
what was seen (its window title, or "works in the background"). Helpers, game stores and programs Windows started
by itself in the meantime are listed unticked.

**Add a program that is not listed:** type its name as Task Manager shows it (without `.exe`) and choose **Add
name**, or **Browse...** to its file. **Find programs in a folder...** offers unticked suggestions to review.
**Learn by opening this card...** (under the fold-out below the list) opens the card, lets you look, and lists
every program that appeared; tick the ones that belong to the game.

**Advanced: let only one program end the game...** adds a column **Ends the game**. Use it for a launcher with
several games: for E6 Multisport only **E6 Product Launcher** ends the game, so a sport's **Exit Game** goes back
to the launcher's menu and not to the cards. Sports and other helpers close before the launcher; give programs at
least 30 seconds to close. A program that ends the game must also be ticked to close. With nothing ticked at all,
BayLauncher closes the programs the card opens.

Keep firmware updaters, maintenance and configuration tools, crash reporters, system programs, programs that run
as administrator and unrelated background utilities off the list. Leave the wider **also close any other
program** cleanup (advanced editor) off unless you deliberately need it. Setups and Learn never turn it on.

#### Review and try it

The last page says in plain words what the card does: what opens when a guest taps it, in order; the clicks it
makes; and what closes when the game ends. **Try this card...** starts the real programs exactly as a guest's tap
would. Check a normal quit, the back-to-games button, and a second start. For E6, a sport's **Exit Game** must
leave its launcher menu open; ending the session closes the sport before the launcher.

A window appearing does not prove the game is connected or ready to play. Check that in the game yourself,
and read any problem reported by the test. Finish the test and close its game before saving. **Save card** applies
the draft only after validation and a successful settings save. **Cancel** leaves the saved cards unchanged.

### Edit, copy and undo

Select a card in Settings > Cards and choose **Edit with guide...** to use the same pages for an existing
card. **Duplicate** opens a separate draft based on that card with a suggested new name; review its name and
settings before saving. Use **Move up** and **Move down** to change carousel order, or **Delete** to remove a card
after confirmation. Deleting a card does not uninstall its game.

**Made one card per program?** A card for the launch monitor's software and another for the game cannot both
run. Select the card that should open first, choose **Combine...** and pick the other card. The combined card
opens in the guided builder: the first card's programs, then the second's; everything either card closed; each
card's clicks with its own programs. Check it, try it, and **Save card**. Only then does it replace the first
card, and the second card is removed. **Cancel** changes nothing.

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

### Extra apps with a card

Extra apps are optional. You can open a recording app such as OBS, a chat window, a browser, or another supported
app alongside the game. These are examples, not the only choices. Keep the game's own opening and closing group
separate from optional companions.

1. Start with a working game card. To keep that card simple, choose **Duplicate**, then name the copy something
   guests recognise, such as **Golf + Video** or **Golf + Chat**.
2. In **Programs to open**, expand **Also open another app (optional)** and choose **Add app or website…**.
3. In **Choose what to open**, enter a name and choose **App or website in my normal browser** for an ordinary
   program or browser link. Choose **Website panel (Preview)** for the separate built-in website window below.
   Extra program arguments are for ordinary apps that need them, not website panels.
4. **Screen, size and position:** choose how the supported app's window should open. Read the mode's capability note;
   a normal browser link and its manual PiP controls are different from a built-in website panel.
5. **Opening and closing:** choose when it starts and both closing choices explained below.
6. Choose **Apply to card draft**. This returns the changes to the card builder; it has not saved the card yet.
   Review and choose **Try this card…**, finish the test, then choose **Save card**.

Use **Edit app and layout…** to adjust an extra or **Remove** to take it out of this card. Removing an entry does
not uninstall or close its app. **Cancel** leaves the card draft as it was before that editor opened. Changing a
duplicate does not change the original card.

For example, Multisport can remain on the projector while entertainment uses an otherwise unused TV. An OBS
companion opens OBS itself; opening it does not start recording or streaming, or automatically extract its preview.
A chat companion is an ordinary app window. Sign-in, playback, recording and game readiness remain things to
check in those apps.

#### A website in a floating panel

Choose **Website panel (Preview)**, then paste the site's full `https://` address into **Website address**. Use the
normal website, such as a sports provider's watch page; this is not a replacement subscription or a universal video
player. One built-in website panel can be configured on a card in this first version. If an earlier panel was deliberately
kept open, close that panel before starting a different panel card: the new card leaves an already-open helper alone.

Website panels require **Close every new app** to be off in the card's advanced settings, with browser programs kept out of the old opening, closing, ender and pre-close groups. This keeps the **Open in browser** fallback separate from the card's automatic cleanup.

On **Screen, size and position**, choose the projector or TV. **Show website above the game (floating)** is selected initially: it
requests a window above ordinary game windows. Choose a corner and adjust its size, then check the illustration.
If the intended screen is not selected, choose it explicitly. For a website on the other screen without floating
above its windows, choose **Normal website window** instead.

The initial closing choices open the panel after the main card starts, leave golf running if the panel exits, and
ask the panel to close normally when the card ends. Review those choices, choose **Apply to card draft**, test the
whole card and **Save card**. The saved screen, size and position belong to that card. No Windows setting or separate
window-pinning utility is needed to request this layout.

The panel has its own address field, **Go**, **Back**, **Reload**, **Copy link**, **Open in browser** and **Close**. Move and resize
it as an ordinary window. Its own controls remain outside the webpage. Opening a website does not automatically
turn it into video-only PiP; use the site's normal playback controls and test its fullscreen button within the panel.
A Play click may still be needed. Changing the displayed page does not replace the card's saved website address. If **Keep this app open** is selected, the built-in panel can remain after golf ends while
BayLauncher is still running; it closes if its verified BayLauncher owner exits or becomes unavailable.

#### Sports and streaming websites

YouTube, Netflix, NFL services and other sports providers are examples to try, not a supported-service list. Their
sign-in, subscription, location, device and protected-video rules still apply. A page can open successfully while its
video cannot play. Google account sign-in is not supported in this embedded web panel; other services may also need
a normal supported browser. Use **Open in browser** if the panel cannot handle the site. That opens the regular
browser route; its window layout, native PiP and closing remain manual.

The panel does not open website popups, downloads or JavaScript alert/confirm/prompt dialogs. It asks before granting a website permission. Some legitimate
TV sign-in or location checks depend on those capabilities and may need the normal browser. If WebView2 Runtime is
missing or the panel cannot start, read its message and use **Open in browser** or close it. A Microsoft download-page
button is available when the runtime is missing; the panel does not install it automatically. The game can
continue. Neither a panel-start result nor a returned cards screen proves playback or a successful sign-in.

### Saved layouts and floating windows

The companion editor offers these window choices:

- **App chooses:** leave the app's own size and position alone.
- **Saved app window:** choose a screen and a size/position to restore when this card starts, where the app supports it.
- **Floating app window:** use a supported app or built-in website panel above ordinary windows, with the card's
  saved size and position. It is not a target-specific guarantee over only one named program.
- **Browser picture-in-picture (manual):** use the browser's floating video controls. BayLauncher does not automatically
  set that panel's screen, size or position, or close its browser for you.

The built-in website panel can use saved or floating placement. An external website link opens in the normal browser
and has no automatic saved-window placement or browser closing.

For a saved or floating window, choose **Screen**, then adjust **Width**, **Height**, **From left** and **From top**.
The screen illustration and corner buttons help you place it. You can drag the illustration or use the controls
with the keyboard. The percentages describe the selected screen's available area, so the layout can adapt when its
resolution changes. Every card keeps its own layout after **Save card** succeeds.

An already-running or protected app is left alone. BayLauncher may be unable to move an app that manages its own
window or uses a shared browser process. Read the result instead of assuming that opening the app also restored its
layout. If the saved screen is unavailable, its optional extra is skipped and the saved layout is kept; it is not
silently moved over golf. Edit the companion to choose another screen, then try and save the new choice.

Moving an app during play does not silently replace its saved card layout. To change the saved layout, edit the
card, adjust its companion, apply the draft and save the card. Cancelling the editor discards draft changes; it
cannot undo a manual move you have already made in another app.

#### Watch video while you play

For the built-in route, add **Website panel (Preview)** to the card as explained above. BayLauncher can request
its saved screen, size, position and floating mode without the browser's PiP menu. The full website stays available;
actual video, account access and controls depend on that provider.

For the normal-browser route, open the video in a supported browser, start playback and use that browser's
**Picture-in-picture** command. Drag and resize its floating panel, then click back into golf. Closing the PiP panel
can leave the browser open, and hiding it does not necessarily stop playback. BayLauncher does not automatically
restore a normal browser's PiP position.

Floating windows need a compatible game display mode. If the game covers the extra window, try the game's own
windowed or borderless mode and test it again. BayLauncher does not change that game setting for you. Check that you
can return to golf after using the video's controls and that the game still plays smoothly. Keep the normal desktop
escape directions available while testing.

### What closes with a companion app

The two choices are independent:

1. **When this app exits:** **Leave the other apps running** keeps golf and the other companions going. **End this card and close its selected group**
   asks to end the game and close the selected group after BayLauncher observes this owned app actually exit.
   Minimising a window, hiding a video panel or returning a PiP video to its tab is not necessarily an app exit.
2. **When this card ends:** **Keep this app open** leaves the companion running. **Ask this app to close normally** asks a
   supported app started by this card to close normally. It does not force a recording app to stop or dismiss its prompts.

For example, you can choose: "Closing OBS leaves golf running; ending golf asks OBS to close." Another choice is:
"Closing this companion ends the card; ending the card leaves this companion open." Review both sentences before
saving. Unsupported automatic close or exit tracking is unavailable; a browser opened through a website link is
left open for you to manage. Personal windows that were already open and protected Windows/browser programs stay
untouched.

If an app remains open after a normal close request, review its prompt or finish that work yourself. An open app
does not prove that a recording was saved, and a returned cards screen does not mean every companion was closed.
Keep-open results and could-not-close results describe different outcomes. BayLauncher also requests restoration of
window presentation that it changed, so keeping an app open is separate from keeping it pinned above other windows.
If that cleanup cannot be confirmed, use **Retry companion cleanup** and read its result. That action can restore a
kept-open app's presentation without closing it.

#### Check the whole combination

Use **Try this card…** once you have reviewed the draft. Confirm the game's connection and playable screen, the
companion's screen/size/position, and actual playback or recording separately. Then check a normal game exit, the
back-to-games button and the companion's own exit choice. Start the card again yourself to check that its saved
layout restores. Stop the test before saving. A placement result is not a playback or launch-monitor connection check.

### Learn: add the game's programs to the close list

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

### Test card: check a full visit to this game

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

### Advanced settings and safe close lists

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

## Chapter: Recipe: GSPro with ProTee AutoStart

For bays with a ProTee VX that start GSPro through ProTee Labs. ProTee AutoStart is a free BA Custom Products tool that
clicks through ProTee Labs and GSPro to the range by itself:
[Protee-VX-Gspro-Smart-Start-up on GitHub](https://github.com/DiyGolfGuy/Protee-VX-Gspro-Smart-Start-up).

### Before you start
- GSPro opens normally from ProTee Labs on this PC.
- ProTee AutoStart is installed. Turn off its own "start with Windows" option, and in Task Manager > Startup apps
  disable it, so it only runs when the card starts it.
- Neither ProTee Labs nor GSPro is set to "Run this program as an administrator" (right-click the program > Properties >
  Compatibility). BayLauncher cannot close a program that runs as administrator.

### The card

1. Settings > Cards > **Add card**. Give it a name such as "GSPro" and choose a picture.
2. On **Programs to open**, choose the GSPro with ProTee AutoStart recipe and browse to ProTee AutoStart's program.
   Its one open step uses **Arguments** `/run` (skips AutoStart's 5-second countdown), **Wait for** `GSPro`, and
   **Timeout (s)** `660` (AutoStart gives up after 600 seconds; this allows a minute more). Do not add another open
   step for ProTee Labs or GSPro when AutoStart already opens them.
3. On **Programs to close**, keep GSPro, `GSPconnect`, ProTee Labs and AutoStart in the closing group. Use
   **Learn by opening this card...** to review anything else this bay starts. `GSPconnect` has the window title "ProTee United VX"; if
   it stays open, ProTee Labs can think GSPro is still running on the next launch.
4. Check the ender choices. Exiting GSPro should finish the session; if exiting ProTee Labs is also meant to end it,
   make it an ender too. Keep the connector and any short-lived helpers as close-only rows.
5. **Review and try it** > **Try this card...**, then finish the test and **Save card**.

A working close list looks like: `GSPro, GSPconnect, ProTee Labs, ProTeeAutoStart`. If AutoStart runs as an AutoHotkey
script, it shows as AutoHotkey (for example `AutoHotkey64`) instead.

### Check it

Expect **Opening GSPro**, then the GSPro window. Check the ProTee connection and reach the range yourself: a window
wait does not check those. Quit GSPro normally and check that the connector, ProTee Labs and AutoStart close too.
Open again and quit ProTee Labs if you made it an ender. Finally open again, press the back-to-games button and
choose **Yes, end it**. Each route should bring the cards back, and the next launch should work without clearing
leftovers by hand. Leave the card unchanged if a known working bay uses a different program name; check its actual
programs before changing it.

---

## Chapter: Recipe: TruGolf Multisport

For TruGolf's E6 Product Launcher, where each sport is its own program. Leaving a sport (Exit Game) should go back
to the launcher's menu, and only closing the launcher should bring the cards back.

### The card

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

### Finding the sports' program names
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

### Check it

Open the card, start a sport and use **Exit Game**: expect the launcher's menu, with no BayLauncher cleanup of that
menu. Close the launcher: expect the cards back. Start a sport again and use the back-to-games button: expect the
sport and its game helpers to close, then the launcher, then the cards. Open the card once more to check that it
starts normally and TruGolf's activation is still intact. A sport returning straight to the cards usually means
it was made an ender, or no explicit launcher ender was set.

---

## Chapter: The back-to-games button

During a game, one button ends it: a key combo on a keyboard, or a button on a BA control box (or any box that sends a
key).

### Set it
1. Settings > **General** > Back-to-games combo > **Change...**.
2. Press the keys (or the control-box button) you want. BayLauncher shows what it captured.
3. **Save**. The combo works from then on. (A new bay starts with Ctrl+Alt+Home.)

### Use it
- Press it during a game: **End this game?** appears, with **Yes, end it** and **No, keep playing**.
- Press it a second time, or choose **Yes, end it**: everything on the card's close list closes and the cards come back.
- No answer: the question closes by itself after a few seconds (Settings > General) and the game keeps running.

---

## Chapter: Screens and the look

### Screens
Settings > **Screens** lists every screen Windows knows.
- **Identify all screens** shows a big number on each screen, so you know which is which.
- Select the screen that should show the cards and press **Use for the carousel**. It is saved and used at once.
- In the free edition, every screen uses the built-in background selected in **Look**. Classic BA Custom Products
  keeps the original whole artwork, faded on side screens and darker behind the cards, so its QR code stays readable.
  The other backgrounds fill the screen and retain a small BA logo, name and bacustomproducts.com advertising panel.

### The look
Settings > **Look** changes how the cards look. Try options and watch the preview; nothing changes on the cards
screen until you press **Use this look** (**Undo** goes back).
- **Free background**: Classic BA Custom Products, three photo-style scenes (Midnight simulator, Golden-hour
  links, Mountain valley) and six drawn backgrounds in full 4K (Green contours, Night range, Dusk hills, Ball
  close-up, Yardage book, Fairway stripes). The preview shows your choice. **Use this look** saves it for the cards and side screens; **Undo** discards unsaved look
  changes. Free backgrounds keep BA advertising; custom background uploads remain an Owner/unlocked feature.
- **Layout**: Carousel (big middle card), Row (all cards the same size), or Grid (rows of cards).
- **Card size**: Small, Medium or Large.
- **PIN pad style**: Classic, Round (phone style) or Minimal.
- **Highlight colour** for the selected card and the PIN pad's OK key.
- **Show the "click to play" hint** under the cards.

---

## Chapter: Turning BayLauncher on and off for an account

"On" means this Windows account starts straight into the cards at sign-in, with no desktop or taskbar. It is set for
one account at a time. Use the account the bay signs in with.

### Turn it on
1. Sign in to the bay's account.
2. Start > BayLauncher > **Turn on BayLauncher for this account**. A window lists what it did, and a
   **Restore Windows Desktop** shortcut appears on that account's desktop.
3. Sign out and sign back in. The cards fill the screen.

### Turn it off
1. Get to the desktop (see [Getting back to the Windows desktop](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/back-to-the-desktop.md)).
2. Run **Restore Windows Desktop** (the desktop shortcut, or Start > BayLauncher). It is safe to run twice.
3. The next sign-in is the normal Windows desktop.

### While it is on
- If BayLauncher is closed or crashes, it starts again by itself. If that happens three times within two minutes, the
  normal desktop starts instead, until the next sign-in.

---

## Chapter: Getting back to the Windows desktop

There is always a way back. Keep this page handy for staff.

1. **Staff PIN**: the lock button (top right) > PIN > **Desktop**. After 10 minutes without anyone using the PC, a one-minute
   countdown shows, then the cards come back by themselves. Move the mouse to stay. Nothing you opened is closed.
2. **Ctrl+Alt+Del** > Task Manager > **Run new task** > type `explorer.exe` > OK. The full desktop and taskbar appear.
3. **Restore Windows Desktop** (desktop shortcut, or Start > BayLauncher): turns BayLauncher off for this account from
   the next sign-in.
4. **SAFE.txt**: create an empty file named `SAFE.txt` in `C:\ProgramData\BayLauncher`, then sign out and back in. You
   get the normal desktop. Delete the file and sign in again to go back to the cards.

### The staff PIN
- 4 to 8 digits. After 5 wrong tries the PIN pad locks for 5 minutes.
- Change it in Settings > General > **Change the staff PIN...**.
- The PIN pad closes by itself after 30 seconds without input.
- **Forgot it?** From the desktop (way 2 above), choose Start > BayLauncher > **Reset the staff PIN** and type a new
  one twice. The cards use it within seconds.

---

## Chapter: Moving your settings to another bay

Settings > **Tools** > **Export settings and pictures...** saves one file with your cards, look, screens, staff PIN and
pictures. On the next bay: Settings > Tools > **Import settings and pictures...** and choose that file.

After importing, check each card's program locations: a program installed in a different folder on the new PC must
be chosen again with **...**. Screens are matched by Windows' screen names, so check Settings > Screens too.

---

## Chapter: Troubleshooting

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

**A second card will not open while a game is running**
- Only one card runs at a time. Put everything a game needs (the launch monitor's software, any connector and the
  game) on one card: see [Cards and Learn](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/cards-and-learn.md).

**The start-up clicks stop, or a click comes too early**
- Settings > Cards > **Edit with guide...** > **Clicks to get in** shows every click with its picture.
  **Test card...** says which click stopped and why; the log has the same line.
- "The screen never showed ..." or "The screen never looked the way it did when the click was recorded": the
  game's menu changed (often after an update) or a notice came up. The log line lists the words BayLauncher read
  and names a picture of what it saw in the logs folder. Use **Teach this click again...** on that click, or add
  the notice's button words under **Notices to click away**.
- A click that comes too early: on **Clicks to get in**, make **Wait before this click** longer for that click, or
  make the settle time at the top of the page longer (one second is the start).
- "Windows did not accept the click": the program runs as administrator. Turn that off in its
  Properties > Compatibility.

**The back-to-games button does nothing**
- It only works while a game from a card is running. Check the combo in Settings > General (**Change...** and press
  the button again).

**The bay starts to a black screen**
- Use Ctrl+Alt+Del > Task Manager > Run new task > `explorer.exe`, then see
  [Getting back to the Windows desktop](https://github.com/DiyGolfGuy/BayLauncher/blob/main/guide/back-to-the-desktop.md).

**Forgot the staff PIN**
- Get to the desktop with Ctrl+Alt+Del > Task Manager > Run new task > `explorer.exe`, then Start > BayLauncher >
  **Reset the staff PIN**.

**Where are the logs?**
- Settings > Tools > **Open the logs folder** (`C:\ProgramData\BayLauncher\logs`). One file per day, kept 30 days. They
  record what BayLauncher did, never the PIN.

---

## Chapter: Privacy and safety

### What BayLauncher does not do
- BayLauncher keeps its settings, card pictures and logs on this PC and has no built-in HTTP upload of those files.
  Optional companion apps and websites that you choose to open can use the network and their own accounts and privacy
  settings. BayLauncher does not inspect their page, chat, video or recording content.
- It sets no Windows policies, blocks no keys and installs no services or drivers.
- It does not alter the games' files or settings. It starts their configured programs and follows their closing
  choices; optional companion layouts can move and resize supported windows.
- Day to day, nothing runs as administrator.
- It makes mouse clicks only on cards where staff recorded start-up clicks, only inside those cards' programs, and
  only while such a card starts. **Watch me start it** notes which programs start (their file locations and
  start-up options) and where the left mouse button is clicked, from the moment staff start a recording until
  **Ready** or **Cancel**. It does not read the keyboard, uses no keyboard or mouse hook, and never blocks input.
  Small pictures of the clicked spots are kept with the card pictures on this PC.
- To know when a game's screen is ready, it reads the words in the windows of the card's own programs with the
  text reader built into Windows, on this PC: while staff record or teach a click, and while such a card starts.
  Only the words of the clicked screens are kept in the card. Nothing is sent anywhere.

### What it stores, and where
- The program: `C:\Program Files\BA Custom Products\BayLauncher`.
- Settings, card pictures and logs: `C:\ProgramData\BayLauncher`. These files have no built-in network upload.
- The optional website panel requests a private browsing session and uses its own folder for each run under
  `%LOCALAPPDATA%\BA Custom Products\BayLauncher\WebsitePanelPreview\profiles`. It never borrows or copies a personal
  Edge or Chrome profile. Local browser folders can remain after closing; this is not a secure-erasure feature.
  Use **Open in browser** only when you intend to use that normal browser's own profile and sign-in. Consider who
  uses that browser before signing into a shared bay PC.
- The staff PIN is stored only as a salted hash, never as the digits. Logs record each PIN attempt, never the digits.
- When a start-up click cannot be made, a picture of that program's window as BayLauncher saw it, in the logs folder
  (`click-not-made-...jpg`; the newest ten are kept), so staff can see what went wrong.
- A Bay ID for this PC (Settings > About and the log): made from the motherboard's and the system disk's serial
  numbers with a one-way hash. The serial numbers themselves are not stored. It stays on the PC.

### What it changes in Windows
- Only when you choose **Turn on BayLauncher for this account**: that one account's sign-in program (its "shell"
  setting) points at BayLauncher, and a **Restore Windows Desktop** shortcut goes on that account's desktop.
  **Restore Windows Desktop** puts it back.
- A Start menu folder, BayLauncher, and an entry in Settings > Apps > Installed apps.
- Every account on the PC may write to `C:\ProgramData\BayLauncher` (a folder permission set when installing), so
  settings can be saved without administrator rights.

### Programs it never closes
Windows' own programs (Explorer, Task Manager and everything in the Windows folder), command and PowerShell windows,
Python programs, shared Microsoft Edge/WebView2 processes and programs that run as administrator stay outside the
normal game cleanup. BayLauncher can normally close its own website-panel window and release that window's browser
control; it does not force-kill every Edge or WebView2 process. Anything already running before a card was clicked
is not closed by the "also close any other program" option.

The optional website panel contacts the websites you open and their services, using those sites' own network and
privacy behavior. This is separate from the local launcher settings. A future optional Unlock would have its own
network and privacy explanation before release.

---

## Chapter: Reporting a safety concern

If you think BayLauncher could harm a PC, lock someone out, or behave in a way this guide does not describe, please
contact BA Custom Products through [bacustomproducts.com](https://www.bacustomproducts.com/) and describe what
happened and on which version. Please contact us before posting details publicly, so a fix can go out first.

Only download BayLauncher from the link on bacustomproducts.com or from this page. Each release lists the setup
file's SHA-256 checksum so you can check the file is the one BA Custom Products published.

---
BayLauncher owner guide for AI assistants, version 2026-11-16 (BayLauncher 1.0.8). © 2026 BA Custom Products LLC.
