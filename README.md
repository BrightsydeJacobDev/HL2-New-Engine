# Half-Life 2: reUpdate - 20th anniversary update for HL2: Update
<center><img src="https://github.com/megakarlach/HL2reUpdate/blob/main/hl2reupdatelogo.jpg?raw=true" width="480" ></center>

See this patch showcases here:
https://www.youtube.com/embed/BPhvxuZAkQ4

More information about this patch:

GameBanana: https://gamebanana.com/mods/429040

PCGW: https://community.pcgamingwiki.com/files/file/2588-hl2-update-new-engine-patch-new-bugfixes-for-hl2-update-updated-2023/

GitHub: Go to [Releases](https://github.com/megakarlach/HL2reUpdate/releases).

# Versions

Patch current version: 2.0.0.1 - build 9352380 (20th anniversary + hotfix) - 11/17/2024 (Windows)

Linux version: 1.0.4.1 (tomorrow or next few day I might try to port changes from 20th anniversary)

Based off November 17, 2023 official patch.

# Downloads:

See above (GameBanana/PCGW/GitHub). MEGA LINKS NO LONGER UPDATED.

# About this mod
WARNING: This mod is for "Half-Life 2: Update" (AppID: 290930) only.

This is the unofficial patch for Half-Life 2: Update, which adds all the bug fixes, Steam Deck features from original (vanilla) Half-Life 2 to HL2: Update.

## Installation / Update
See [Wiki - Installation](https://github.com/megakarlach/HL2reUpdate/wiki/Installation)

SINCE 2.0.0.0 UPDATE, YOU MUST UNINSTALL PREVIOUS VERSION (reUpdate 1.x.x.x), AND VERIFY HL2: UPDATE ON STEAM, BEFORE INSTALL ANY NEW VERSION.

(Optional) If you want to install the custom Orange-themed Gamepad UI with Verdana & Trebuchet MS font (inspired by the X360/PS3 Orange Box menu UI),<br>
put the VPK file into hl2\custom folder (if it doesn't exist, create it).

NOTE: For those who don't know where Steam and the game (Half-Life 2: Update) is installed, go to Steam Library > 
right click Half-Life 2: Update > Properties > Local Files > Browse...
An explorer/file browser window will pop-up. Copy the path from the address bar (example: V:\Steam\steamapps\common\Half-Life 2 Update, may vary by system).

## Official Features:
- Increased FOV from 90 to 120
- HUD Aspect Ratio (4:3, 16:9, 16:10)
- Vulkan renderer (-vulkan)
- Classic Old Engine particles
- Working Gamepad UI/Steam Deck UI (-gamepadui), also to use Gamepad UI with DX9, use (-dx9 alongside -gamepadui)
- XInput/Legacy controller support has working rumble/vibration (as SDL2 was updated) (Windows only).
- Steam Input (needs to be enabled on Steam client)

Beside the official changes above. The reUpdate patch also added/changed some features:
- The Gamepad UI have been customized, in this case, most thumbnails on "New Game" chapters are taken from HL2: Update instead of the vanilla HL2.
- More improvements and few new features to Gamepad UI, restored some missing options, including:
  Keyboard Advanced Options:
    Fast Weapon Switch - Disabled (0), Enabled (1), Controller (2), Horizontal scroll/Postal III style (3), can be also changed with "hud_fastswitch" command.
    Enable Developer Console directly via Gamepad UI
    Mouse sensitivity on Gamepad UI can be increased up to 20.
- (NEW) Some improvements to old VGUI:
  Video - Advanced
    Removed broken "Use 'bloom' effect when available" that always uncheck itself when saved. Bloom and HDR will still functioning normally with it's options remain available.
    FOV options increased to 120 without using Console command.
- Optional: Orange Gamepad UI scheme with Verdana & Trebuchet MS font included.

# New since 11/16/2024:
## **HALF-LIFE 2 20th ANNIVERSARY UPDATE**
See changes at: https://www.half-life.com/en/halflife2/20th
## **Other**
- Steam Input seems to be functional, again. To get this to work you need to enable it on Steam > View controller settings.
- Updated SDL to 2.30.9
- Updated DXVK to 2.5
- Updated dxsupport.cfg (again) to includes NVIDIA GPU from GTX 700 series up to RTX 40 series, aswell as forcing dxlevel 95 on Intel HD Graphics.
-- This meant that the game will now set anti-aliasing, textures and other settings to highest on these GPUs by default when launching the game for first time.
-- On other GPUs, the game will default to 4x MSAA, just like the 20th anniversary version.

## Bugs fixed:
November 16/17, 2024 (Hotfix)
- Fixed a crash that could occur in some languages when starting a new chapter.
- UI - Fixed some weapon icon alignment issues at various resolutions.
- Workshop changes not included since HL2 Update never have one anyway.
November 16, 2024
- See changes at: https://www.half-life.com/en/halflife2/20th
- ReUpdate: Fixed Steam Input support. You might need to enable this on Steam first to make sure it's working.

Previously:
- Dropship container gun fix which makes the gun possible to turn (broken since 2007 on X360/PS3, and 2010 on PC. Fixed in 2022.)
- Long loading saves bug/engine freezing while saving has been fixed.
- Improved loading times (for users with HDD only)
- Fixed some stuttering on level transitions
- NPC eyes not blinking (fixed in 2019)
- Some missing Combine sounds has been fixed (noticeable by shooting them)
- and much more... (see [here](https://web.archive.org/web/20160830085422/http://forums.steampowered.com/forums/showthread.php?t=1286478))

# Bugs that hasn't been fixed
- DirectX 8 feature level by default. This is a common bug that also affect vanilla HL2 aswell, when playing the game on some modern hardware/GPUs.
  To workaround this bug, launch the game with -dxlevel 95, configure your video settings, save it (by clicking OK), then
  exit the game, remove the launch options, launch the game again, if your video settings was reset again, just configuring it again, then save it, try to relaunch
  just to make sure, if video settings doesn't reset to low quality, low textures or DX8, then you are good to go.

# LICENSE (ignore)

Games files included in this patch are © 2004 - 2024 Valve Corporation.
Commercial purposes not allowed.

SDL 2 and DXVK:
```
This software is provided 'as-is', without any express or implied
warranty.  In no event will the authors be held liable for any damages
arising from the use of this software.


Permission is granted to anyone to use this software for any purpose,
including commercial applications, and to alter it and redistribute it
freely, subject to the following restrictions:

1. The origin of this software must not be misrepresented; you must not
   claim that you wrote the original software. If you use this software
   in a product, an acknowledgment in the product documentation would be
   appreciated but is not required.

2. Altered source versions must be plainly marked as such, and must not be
   misrepresented as being the original software.

3. This notice may not be removed or altered from any source distribution.

                  Copyright (c) 2017 Philip Rebohle
                  Copyright (c) 2019 Joshua Ashton
                  Copyright (c) 2019 Robin Kertels
                  Copyright (c) 2023 Jeffrey Ellison

                          zlib/libpng license

This software is provided 'as-is', without any express or implied
warranty. In no event will the authors be held liable for any damages
arising from the use of this software.

Permission is granted to anyone to use this software for any purpose,
including commercial applications, and to alter it and redistribute it
freely, subject to the following restrictions:

– The origin of this software must not be misrepresented; you must not
  claim that you wrote the original software. If you use this software
  in a product, an acknowledgment in the product documentation would be
  appreciated but is not required.

– Altered source versions must be plainly marked as such, and must not
  be misrepresented as being the original software.

– This notice may not be removed or altered from any source distribution.
```
Uses Half-Life 2 icon made by vaksa for the setup bitmap.
© 2005 vaksa
https://www.deviantart.com/vaksa/art/Half-Life-2-icon-16869820
and the Windows Vista/7 setup icon from Microsoft Windows. © Microsoft Corporation.

This patch is not made by, or affiliated with Valve, Fillip Victor, and others who have worked on the game.



