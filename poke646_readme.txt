Poke646 and Poke646: Vendetta
Original mods by Marc Schröder / Mindmotor Studios

Version 1.3

Converted for Sven Co-op by Zorbos

Lobby map made by Zorbos
Checkpoint model made by Zorbos
Weapon select HUD icons by Zorbos
AngelScript Programming by Zorbos 
po_c4m6 Anti-Troll Tripmine script made from code by w00tguy123
Player models and portraits made by Zorbos - Based off of pre-existing Sven Co-op models, which are credited to the Sven Co-op team and Valve

The rest of the content is credited to Mindmotor Studios.

Thanks to everyone on the forums who has given me a tremendous amount of help with the AngelScript portion of this release.

====================================================
////////////////////////////////////////////////////
====================================================

DISCLAIMER:

I am not affiliated in any way with the development of Poke646 and Poke646: Vendetta nor do I take credit for any of their contents. I have simply edited the maps so that they work in Sven Co-op.

If you like Poke646 and Poke646: Vendetta, support the creators by downloading and playing the original mods!
Check http://www.poke646.com for downloads and everything related to Poke646.

- Zorbos

====================================================
////////////////////////////////////////////////////
====================================================

TO INSTALL:
Extract to your svencoop_addons or svencoop_downloads directory

Other info:
Survival Mode is enabled by default. If you wish to turn this off, simply edit the map cfg file (ex: po_c2m4.cfg) and add the following:

mp_survival_supported 0 

You can also type this command into the console to disable it during a game.


Poke646 © 2001 and Poke646: Vendetta © 2006 by Marc Schröder and Mindmotor Studios. All rights reserved.

====================================================
////////////////////////////////////////////////////
====================================================

R4to0's fixes:

Changes made for HLDM-BR.NET servers - October 2017
- Moved all music to ambient_music
- Fixed all invalid paths such as global lists

Scrtipt fixes - May 8, 2019

- Added SetThink( null ) on Holster() for heat/lead pipe. Fixes SendWeaponAnim crash issues.
- Removed the remaining old Survival references from po_c4m5 script. Fixes scripts not compiling on po_c4m5 due to missing includes or nonexistent member variables.
- Cast m_pPlayer into EHandle, to prevent any other crashes related to player pointers.

Script changes - May 12, 2019
- Reinstated survival mode and added point_checkpoint script. Survival mode is not enforced and is defined by server's mp_survival_mode cvar. Intro/outros and lobby are explicitly disabled. 
- Disabled antirush on po_c4m2 to prevent running out of time because of map change delay.
- Updated all map cfg files with new survival changes.

Script changes - May 20, 2019
- Added SetThink( null ) on Holster() for sawedoff shotgun. Fixes null pointer access in EjectShell.

Script changes - September 24, 2019
- Added Holster baseclass call to all weapon scripts that override this function. Fixes weapon viewmodel stuck in observer mode (Thanks GeckonCZ).
