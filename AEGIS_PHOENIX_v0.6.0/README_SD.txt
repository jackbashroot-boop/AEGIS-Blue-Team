AEGIS PHOENIX v0.6.0 - BLUE TEAM (defensive sensor) - SD INSTALL
================================================================
For: M5Stack Cardputer ADV with M5Launcher already installed.
This is a DEFENSIVE, receive-only monitoring app. It never transmits
attacks: it watches Wi-Fi/BLE/LoRa/GNSS, logs evidence and alerts you.

WHAT YOU NEED
- Cardputer ADV + microSD card (FAT32) + M5Launcher on the device.

INSTALL (about 2 minutes)
1. Power the Cardputer OFF.
2. Copy the whole folder  AEGIS_PHOENIX_v0.6.0  onto the SD card root.
   (Optional: also copy the contents of SD_ROOT to the card root to get
   starter config/rules. Not required - the app creates what it needs.)
3. Safely eject, insert the card, power on into M5Launcher.
4. Browse into AEGIS_PHOENIX_v0.6.0 and select aegis-phoenix-adv.bin.
5. Confirm the install. If M5Launcher warns it would REPLACE an app you
   still need, stop and free a slot first - do not overwrite blindly.
6. Launch AEGIS PHOENIX from the Launcher like any other app.

VERIFY YOUR DOWNLOAD (optional, on a computer)
sha256sum aegis-phoenix-adv.bin must equal:
4c198134f8b75845bf863dacd3bd59a2facb2fee9744d632ae6a28cf8eaefa97

FIRST 5 MINUTES
- Keys 1-9 jump between views, 0 = logs. Fn+; , . / = arrow keys.
- S = Wi-Fi scan, N = scan your own LAN, W = wardrive mode,
  T = integrity check, P = passive offline mode, Q twice = quarantine.
- Evidence and logs are written under /AEGIS on the SD card
  (AES-256-GCM encrypted forensic log). Take the card out to read them.
- Optional extras it auto-detects: Cap LoRa-1262, GNSS cap, Grove
  ESP32-C5 companion (UART), RFID2 unit. None are required.

NOTES
- App-only binary: install via M5Launcher. Never flash it at address 0
  with esptool, and never write it over a bootloader image.
- To go back, just pick another app in M5Launcher - nothing is erased.
