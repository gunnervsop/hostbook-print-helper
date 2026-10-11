# Hostbook Print Helper

An optional app for a host-stand computer. It lets
[Hostbook](https://www.thehostbook.com) print visit notes to a receipt printer
without the browser's print dialog ("silent printing").

**[Download the newest version for Windows](https://github.com/gunnervsop/hostbook-print-helper/releases/latest/download/Hostbook-Print-Helper-Setup.exe)**
· [All releases](https://github.com/gunnervsop/hostbook-print-helper/releases)

## What you need

- A Windows computer with Chrome or Edge. (iPads, phones and Safari can't run
  it; they keep using the print dialog.)
- A receipt printer that understands ESC/POS (Epson TM, Star in ESC/POS mode,
  Bixolon, Citizen, most 58 mm and 80 mm thermal printers), installed on the
  computer or reachable on the network by IP address.

## Setting it up

1. Download and run `Hostbook-Print-Helper-Setup.exe`. It installs for the
   signed-in person, without an administrator prompt, and opens its window.
2. Choose the printer and the paper width, then **Print a test slip**.
   **Blank lines after each slip** sets how much paper follows a slip.
3. Optional: **Start when I sign in**, so it is ready every day.
4. In Hostbook: ⋯ → Device settings → Visit notes printer → **Silent printing**
   → **Connect to Print Helper**. When Chrome or Edge asks whether Hostbook may
   connect to apps on this computer, choose **Allow**.

If Windows shows "Windows protected your PC", choose **More info → Run
anyway**, or ask IT to allow it. If the helper is closed or can't print,
Hostbook opens the print dialog instead, so no slip is lost.

## Updates

The helper checks for a newer version when it starts and every six hours. When
one is ready, it says so in a notice, in its tray menu and in its window, and
Hostbook's Device settings says so too. Choose **Download update** and run the
installer: it installs over the old version and keeps your printer and
settings. Nothing installs by itself.

## Privacy and security

- It listens only on this computer (`127.0.0.1`) and accepts slips only from
  Hostbook's own addresses.
- Slips go straight to the printer. They are never saved to disk or logged,
  and the settings hold no guest information.
- The update check reads Hostbook's list of releases. It sends nothing about
  the venue or its guests.

## About this repository

This repository holds the Print Helper's releases. Each one is built and
published automatically from Hostbook's source.
