# OpenSesame_4flipper
OPENSESAME SUBGHZ BRUTEFORCE BUNDLE

this ones for desertapple3

inspired by samyk's opensesame attack

⸻
## How the Attack Works

OpenSesame written by SAMYK uses a **Flipper-compatible SubGhz RAW file** to replay a captured garage door signal that was encoded using a fixed binary pattern. These older fixed-code systems operate without encryption or rolling code, making them susceptible to brute-force or replay-based attacks.

The included `.sub` file transmits a sequence that mimics a legitimate remote. If a matching code is received by a vulnerable garage door receiver, the door will open.

---

## De Bruijn Sequence Brute Forcing

Some modern garage door remotes transmit a fixed number of bits (e.g., 12-bit, 18-bit, or 24-bit codes). Instead of manually trying every code one-by-one, OpenSesame can be adapted to use a **De Bruijn sequence**, a mathematical structure that contains every possible combination of bits in a sliding window.

While this base repository contains a single replayable fixed-code signal, future updates may include:

- A full De Bruijn sequence transmitter for known bit-length openers
- A Flipper loop-mode or on-button-press transmitter
- User-selectable De Bruijn segments for popular protocols

---

## Compatibility Notes

This signal targets **older fixed-code garage doors** operating at 390 MHz with OOK modulation. This includes:

- Genie Intellicode (pre-rolling code)
- LiftMaster/Chamberlain units manufactured before ~2006
- Some standalone DIY garage or gate controllers
- Alarm system panels using fixed SubGhz sequences

It will **not work** on systems with:

- Rolling code encryption
- Challenge-response authentication
- Smart garage integrations (e.g., MyQ, Wi-Fi linked)

---

## Ethical Use

This tool is provided for research and educational purposes. Only use on devices you own or are authorized to test. Misuse may be illegal depending on your jurisdiction.


## Firmware Requirements & things you need: 

 - [Unleashed Firmware](https://github.com/DarkFlippers/unleashed)

-  an external CC1101 module
---------

 WINDOWS + MAC INSTALLATION GUIDE

All instructions are 100% identical for both Windows and macOS unless otherwise noted

⸻

STEP 1: Download & Install QFlipper

 1.	Go to:

 https://flipperzero.one/update

 2.	Download QFlipper for your system:

 •	Windows (.exe)

 •	macOS (.dmg)

 3.	Install it like a normal app

 4.	Open QFlipper and plug in your Flipper with USB-C

⸻

 STEP 2: Create Your .sub Files

1. Open Notepad (Windows) or TextEdit (macOS):

 •	On macOS, press Cmd + , in TextEdit → select Plain Text Mode

 •	On Windows, use Notepad or Notepad++

2. Copy the following files from this repository 

3. Save each file:

 •	File > Save As…

 •	Name them:

 •	opensesame_315.sub

 •	opensesame_390.sub

 •	opensesame_433.sub

 •	File encoding: UTF-8

 •	File extension: .sub 

⸻

 STEP 3: Upload Files to Flipper

 1.	Open QFlipper

 2.	Click the file manager

 3.	Navigate to:

/subghz/

4.	Drag & drop your 3 files into that folder

 5.	Wait for upload confirmation

⸻

STEP 4: Launch on Flipper

 1.	On your Flipper:

 •	Go to: Sub-GHz → Saved

 •	You’ll see:

 •	opensesame_315.sub

 •	opensesame_390.sub

 •	opensesame_433.sub

 2.	Choose the one that matches your target’s likely frequency (try all 3 if unsure)

 3.	Stand ~10–30ft from the garage

 4.	Press Send

⸻

### Disclaimer: only use on equipment you have explicit permission to test on. user assumes all risk.

x0x thank you homies for all the continued support x0x
