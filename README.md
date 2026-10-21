# Advanced A-10

A "what-if" mod for the DCS World **A-10C II**: what the Hog might look like with the cockpit and
datalink upgrades the USAF planned for it.

**[Download the latest version](https://github.com/M1344/advanced-a10-releases/releases/latest)**

## Based on the planned A-10 upgrades

Under the A-10 Common Fleet Initiative, the USAF planned to replace the A-10's remaining analog
front-panel instruments with a single display and to add Link 16 next to SADL
([The Aviationist, 2019](https://theaviationist.com/2019/09/10/the-a-10c-warthog-gets-new-upgrades-to-be-ready-to-fight-in-future-high-end-conflicts/)).
This mod is one interpretation of that idea. The display's design is ours: the real upgrade's
look was never made public, and the A-10C in DCS doesn't have any of this.

## What it adds

- **Center display** over the ADI and HSI, with 20 mouse-clickable buttons and a FULL/HALF split
  screen. Pages:
  - **ADI** and **HSI**: driven by the stock instruments, so their modes, failures and the
    HDG/CRS knobs keep working.
  - **SIT**: moving map with your route, bullseye, SAM threat rings and datalink aircraft.
  - **STAT**: datalink status, nearest threats, and whether you're inside a SAM ring.
  - **MFCD repeaters**: copies of your left or right MFCD.
- **TAD**: datalink aircraft (friendly/hostile) and SAM sites with their range rings.

## A simulated datalink, not a god's-eye view

- **Aircraft** appear only when a friendly datalink source would plausibly hold them: an airborne
  AWACS or a flying Link 16 fighter's radar, within range and line of sight. No donors, no
  picture. It's an approximation built from DCS's export data, not DCS's full sensor simulation
  (no terrain masking or jamming).
- **SAM sites** come from the mission plan, like pre-flight intel. Sites spawned later by
  scripts don't appear.

## Good to know

- **Integrity check:** fails while the mod runs (it modifies cockpit files, including adding
  click points to your copy of the cockpit model for the buttons). Use it in single player and on
  servers that don't enforce the integrity check.
- **Multiplayer:** the aircraft picture needs the server to allow object export (the same setting
  Tacview needs).
- **On/off:** the mod is active while the Advanced A-10 tray app is open. Closing it restores
  every DCS file to stock, byte for byte. Nothing of ED's is included in the download.
- **Windows warning:** the installer isn't code-signed yet, so Windows may say "unknown
  publisher" (More info, Run anyway).

## Install

1. Download `AdvancedA10-Setup-<version>.exe` from the
   [latest release](https://github.com/M1344/advanced-a10-releases/releases/latest) and run it.
2. Start **Advanced A-10** (it sits in the system tray), then start DCS.
3. Fly the A-10C II. Button key bindings: Options, Controls, A-10C II, category "Advanced A-10".

**Updates:** the tray app checks for new versions; use "Check for updates" / "Install update".
Updates are signature-checked before they install.

## Coming next

- More of the six-pack on the display: airspeed and altitude tapes, vertical speed and turn rate
  on the ADI page.

Feedback and bug reports are welcome in the
[Issues](https://github.com/M1344/advanced-a10-releases/issues) tab.
