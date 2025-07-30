# Entra Admin Matrix

Gnerates Data Matrix barcodes for LAPS passwords in Microsoft Entra Admin Center. Scan with a barcode reader 
## What it does

- Detects when a password is visible (not hidden)
- Creates a Data Matrix barcode containing the username and password
- Displays it right below the password field

The barcode contains: `.\Administrator` + tab + `your_password`

## Installation

**[Click here to install the userscript](https://github.com/dtyler04/EntraAdminMatrix/raw/main/datamatrix.user.js)**

You'll need a userscript manager like Tampermonkey or Greasemonkey installed in your browser first.

## How to use

1. Install the script
2. Go to Entra Admin Center and view a device's LAPS password
3. Click the eye icon to show the password
4. A barcode will automatically appear below the password
5. Scan it with your phone or barcode scanner

## Security note

The Data Matrix generation code is included locally for security - no external requests are made. The original library is from [datamatrix-svg](https://github.com/datalog/datamatrix-svg) under MIT license.

## Requirements

- Works on: `https://entra.microsoft.com/*`
- Requires: Tampermonkey or similar userscript manager
