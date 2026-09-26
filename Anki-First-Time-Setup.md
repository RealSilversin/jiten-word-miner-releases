# ANKI WORD MINER 0.1.1 - FIRST-TIME SETUP

Capture Japanese words from a game or video and add them to Anki with a
sentence, picture and optional voice clip. No Jiten account or Python needed.

## WHAT YOU NEED
Windows 10/11 (64-bit), desktop Anki, and an internet connection for setup.
The installer is under 50 MB; downloaded dictionaries and models need more
space. Optional voice clips need several GB. Keep Anki open while mining.

## 1. PREPARE ANKI
Download desktop Anki from https://apps.ankiweb.net/ and open your profile.
In Anki, choose Tools > Add-ons > Get Add-ons and enter:

    2055492159

This installs AnkiConnect, which lets the miner talk to Anki on your computer.
Restart Anki afterward. If you have several profiles, open the one you want
to mine into. Create a destination deck such as "Word Miner" if needed.

## 2. INSTALL THE MINER
Extract this ZIP, then run AnkiWordMiner-Setup-0.1.1.exe.
Launch Anki Word Miner from the Start menu when installation finishes.
It installs separately from the Jiten edition.

## 3. COMPLETE THE FIRST-RUN DOWNLOADS
In "Set up Anki Word Miner", click Set up. Wait for the dictionaries and
screen-reading models to finish downloading and indexing, then click Done.

For the simplest first test, leave voice clips off. You can add them later
through Options > Help & about, then choose to open component setup.
If a download fails, retry: completed components are kept.

After setup, text recognition and Japanese dictionary lookup work offline.
Download voice components before going offline if you want voice clips too.
Anki must still be running locally; AnkiWeb sync is separate.

## 4. CONNECT YOUR DECKS
In the miner, open Options > Anki connection & fields.
Leave the AnkiConnect address unchanged for a normal installation.

If you already have Japanese vocabulary decks:
  - Select each relevant note type.
  - Choose its word field (for example, Expression or Word).
  - Choose its reading field if it has one.
  - Click Use this mapping for each note type.
Use fields containing one vocabulary term, not a sentence or a word list.
Leave Scan all decks enabled unless you want a smaller scan scope.
Click Save & reconnect / scan.

If you have no existing vocabulary decks, you can keep the default mapping.
On Words & queue, choose your destination in Study deck. You can also create
one using Create destination deck in the Anki settings window.

## 5. CAPTURE YOUR FIRST WORD
Open a game or video with visible Japanese text.
In Options > Capture source, select its window. A selected screen region
can be useful when you want only the video picture, without browser borders.
Return to Words & queue and check the Source name and Study deck.

Press Capture now (F10). Review a queued word, its sentence and picture,
then click Add to Anki. Check the resulting card in Anki's Browse window.
Words already found in your mapped decks are normally kept out of this queue.

For continuous capture, turn on Live view and Auto Queue New Words.
You do not need to press Capture now as well. Auto Queue New Words collects
suggestions; you still approve new cards before they are added to Anki.

## OPTIONAL: VOICE CLIPS
Complete voice setup, then enable Capture voice clips on Words & queue.
PC audio records the sound your computer plays. Only captured window targets
the selected window's application (Windows 11); windows or tabs sharing the
same process may also be included. Double-click a word, or press P, to play
its saved voice line. Click the picture to open it.

## OPTIONAL: UPGRADING EXISTING CARDS
You do not need this for ordinary mining. Try adding new cards first.

To enable reviewed-card replacements, install the included companion:
  1. In Anki: Tools > Add-ons > Install from file.
  2. Select AnkiWordMiner-Replacements.ankiaddon from:
     %LOCALAPPDATA%\Programs\AnkiWordMiner
     (Paste that path into File Explorer to find it.)
  3. Restart Anki.

In the miner's Card upgrades tab, enable Upgrade existing Anki cards with
mined cards. Select eligible decks and card templates that test the same
recognition skill. Approve proposals there; automatic approval starts OFF.

The reviewed card continues with mined content, keeping its review history
and scheduling. Original content stays on a suspended card in its old deck.
Use Replacement history to reverse the change, keeping newer review progress.
Keep both notes. Initially, only active review cards are supported; source
and destination decks must use the same options preset and retention settings.

## IF SOMETHING DOES NOT WORK
Cannot connect: keep the correct Anki profile open, check AnkiConnect is
installed, restart Anki, then use Save & reconnect / scan in the miner.

No words appear: check the capture window/region and visible Japanese text.
Known words and filtered text are skipped. Live view needs Auto Queue New
Words enabled to offer new words.

Waiting for a picture: leave Live view running so the miner can confirm the
video crop, or select a screen region. With screenshots enabled, a card waits
for its picture instead of being sent without one.

Downloads/setup: reopen setup from Options > Help & about and retry.

Your settings, mined media and field-change backups are stored in:
    %LOCALAPPDATA%\AnkiWordMiner
Updates and uninstall preserve this data. Replacement backups also live in
anki-miner-replacements.sqlite3 beside your Anki profile's collection; these
local backup files do not sync through AnkiWeb.

Latest downloads:
https://github.com/RealSilversin/jiten-word-miner-releases/releases

The installed Read me has more detail. Main miner application code is
compiled; the optional Anki add-on and some third-party runtime files include
Python. Not affiliated with Anki or jiten.moe.
