# JITEN WORD MINER 0.1.1 - FIRST-TIME SETUP

Capture Japanese words from a game or video and add them to your Jiten deck
with a sentence, picture and optional voice clip. No Python, Anki or Jiten
Audio Manager installation is needed.

## WHAT YOU NEED
Windows 10/11 (64-bit), a Jiten account, and an internet connection.
The installer is under 50 MB; first-run models and optional voice components
are larger downloads. Jiten lookups and card uploads require the internet
even after setup. For offline mining into Anki, use the separate Anki edition.

## 1. INSTALL THE MINER
Extract the download ZIP, then run JitenWordMiner-Setup-0.1.1.exe.
If you downloaded the installer directly, just run it.
Launch Jiten Word Miner from the Start menu when installation finishes.
It installs for your Windows user and keeps its data separate from Anki.

## 2. COMPLETE THE FIRST-RUN DOWNLOADS
In the setup window, leave voice clips off for a simpler first test, then
click Download. Wait for the screen-reading models and any required NVIDIA
components to finish. Without an NVIDIA card, screen reading uses the CPU.
Click Done when setup finishes.

You can return later through Options > Help & about > Set up.
If a download fails, retry: completed components are kept.

## 3. CONNECT YOUR JITEN ACCOUNT
Sign in at https://jiten.moe/ and open Settings > Advanced > API Key.
Choose Generate and copy the key immediately: Jiten shows it only once.

In the miner, open Options > Jiten account / API key.
Paste the key and click Save and connect. The miner stores it encrypted
for your Windows user. Keep the key private; do not put it in screenshots.

On Jiten, create a manual study deck of the "word list" type if needed.
In the miner's Words & queue page, select it under Study deck.
The miner needs a writable word-list deck, not a media deck.

## 4. CHOOSE WHAT TO CAPTURE
Open a game or video with visible Japanese text.
In Options > Capture source, select its window. You can also select a screen
region if you want to capture only a video picture, without browser borders.

On Words & queue, check the Source name. Detect fills it from the window
title when possible; turn Detect off and type a title if you prefer.
The source is saved with the mined words.

## 5. ADD YOUR FIRST WORD
Press Capture now (F9) while Japanese text is visible.
Select a queued word and check its sentence and picture.
Click Add to deck (or press A), then check the card on Jiten.

Known words and filtered text are normally skipped. Skip this time leaves
the word available for another capture. Filter in miner keeps it out of
future suggestions; its arrow menu also offers Jiten learning-state actions.
The rarer text-correction controls are under Advanced.

For continuous capture, turn on Live view and Auto Queue New Words.
You do not need to press Capture now as well. Auto Queue New Words collects
suggestions; it does not approve new cards for you.

## OPTIONAL: VOICE CLIPS
Reopen setup and select voice clips. These require several GB of additional
downloads. The voice helper downloads automatically; you do not need to
unpack the separate Voice ZIP yourself during normal setup.

Enable Capture voice clips on Words & queue. In Options, PC audio records
the sound your computer plays. Only captured window targets the selected
window's application on Windows 11; other windows or tabs sharing that
process may also be included.

Double-click a word, or press P, to play its saved voice line.
Click its picture to open it. Finding voice lines is slower on CPU-only PCs.

## OPTIONAL: CARD UPGRADES AND RESTORING CONTENT
Card upgrades reviews captured lines for words already in your Jiten deck.
Select a proposal to inspect its picture and sentence, then Approve card,
Approve all, or Reject card. Automatic upgrades are a separate option on
this page; leave them off while trying the program.

Custom images/audio from other sources are protected unless you explicitly
enable their replacement under Advanced. Before changing existing card
content, the miner saves a local backup; a failed backup blocks the change.

In Mined cards, search for the word and use Review restoration to restore
saved content. Review progress is not rolled back. Backups cannot recover
content overwritten before the miner began saving them.

If you mark a bad line with a standalone x at the start of its note on Jiten,
use Remove all x-flagged lines in Mined cards to process those flags.
This happens when you click the button, not continuously in the background.

## IF SOMETHING DOES NOT WORK
Cannot connect: check your internet connection, reopen Jiten account / API
key in Options, and use Save and connect with a valid key.

No destination deck: create a manual word-list deck on Jiten, then reconnect.

No words appear: check the capture window/region and visible Japanese text.
Known words and filtered text are skipped. Live view needs Auto Queue New
Words enabled to offer new words.

Waiting for a picture: leave Live view running so the miner can confirm the
video crop, or select a screen region. With screenshots enabled, a card waits
for its picture instead of being sent without one.

More detail: Options > Help & about provides setup help and the log folder.

## YOUR DATA AND UPDATES
Settings, queue, pictures, clips and card-content backups are stored in:
    %LOCALAPPDATA%\JitenWordMiner
Updates and uninstall preserve this folder. Keep the whole folder, including
card-history, when backing up your mining data. Backups are local and tied
to the API key used; changing keys does not migrate old backups automatically.

Latest downloads:
https://github.com/RealSilversin/jiten-word-miner-releases/releases

The installed Read me has more detail. Main miner application code is
compiled; some third-party runtime components include Python files.
Not affiliated with jiten.moe.
