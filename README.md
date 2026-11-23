# Desk Pet

Firmware updates and the Mac app for the Desk Pet: a little robot face and clock
on an ESP32-C3 with a 0.96" OLED. Pets with Wi-Fi find new versions here by
themselves and offer the update.

## Downloads

Everything is on the [latest release](https://github.com/DadaSauce/DeskPet/releases/latest):

| File | What it is |
|---|---|
| `Desk_Pet_Mac.zip` | the Mac helper, **Desk Pet.app** (menu bar) |
| `OLED_Keys_C3.ino.bin` | firmware for the Desk Pet with keys |
| `OLED_Face_C3.ino.bin` | firmware for the plain Desk Pet (when released) |
| `latest.txt` | what the pets read to see if they're up to date |

## Docs

- [Quick start](Docs/Desk_Pet_Quick_Start.pdf) - two pages
- [User guide](Docs/Desk_Pet_User_Guide.pdf) - every menu, setting and command

## Installing the Mac app

1. Download `Desk_Pet_Mac.zip`, unzip it, and drag **Desk Pet** to Applications.
2. Open it. The app isn't signed by Apple, so macOS stops it the first time:
   click **Done**, open **System Settings › Privacy & Security**, scroll down
   and click **Open Anyway**. You only do this once.
3. If macOS says the app **is damaged and can't be opened**, run this in
   Terminal, then open it again:
   ```
   xattr -cr "/Applications/Desk Pet.app"
   ```

## Updating a pet

When a new version is out, the pet shows a small arrow at the top left.
Install it from the pet (**Settings › UPDATE › #**) or from the Mac app
(**Settings › Firmware › Install**). Settings, Wi-Fi and pairings are kept.
