# Desk Pet

Firmware updates and the Mac app for the Desk Pet: a little robot face and clock
on an ESP32-C3. There are three pets: the OLED Desk Pet with keys, the plain OLED
Desk Pet, and the round colour Desk Pet. Pets with Wi-Fi find new versions here
by themselves and offer the update.

## Downloads

Everything is on the [latest release](https://github.com/DadaSauce/DeskPet/releases/latest):

| File | What it is |
|---|---|
| `Desk_Pet_Mac.zip` | the Mac helper, **Desk Pet.app** (menu bar) |
| `OLED_Keys_C3.ino.bin` | firmware for the Desk Pet with keys |
| `OLED_Face_C3.ino.bin` | firmware for the plain OLED Desk Pet |
| `DeskPet_Round.ino.bin` | firmware for the round colour Desk Pet |
| `latest.txt` | what the pets read to see if they're up to date |

## Docs

Each pet has its own quick start (two pages) and user guide (every menu, setting and command):

| Pet | Quick start | User guide |
|---|---|---|
| Desk Pet with keys | [Quick start](Docs/Keys/DeskPet_Keys_Quick_Start.pdf) | [User guide](Docs/Keys/DeskPet_Keys_User_Guide.pdf) |
| Desk Pet (plain OLED) | [Quick start](Docs/OLED/DeskPet_OLED_Quick_Start.pdf) | [User guide](Docs/OLED/DeskPet_OLED_User_Guide.pdf) |
| Desk Pet (round) | [Quick start](Docs/Round/DeskPet_Round_Quick_Start.pdf) | [User guide](Docs/Round/DeskPet_Round_User_Guide.pdf) |

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

When a new version is out, the pet shows a small up-arrow (at the top left on
the OLED pets, a green one at the top on the round pet). Install it from the Mac
app (**Settings › Firmware › Install**), or on the pet with keys from
**Settings › UPDATE › #**. Settings, Wi-Fi and pairings are kept. Each pet has
its own version numbers and only ever gets its own firmware.
