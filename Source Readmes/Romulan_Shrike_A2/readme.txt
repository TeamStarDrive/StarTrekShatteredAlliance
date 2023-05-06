*******************************************************************************************
* Model Credits:
*  Romualn Shrike v1.0
*    -  Game: Star Trek Armada II
*    -	Mesh Developer: Achilles
*    -	Texture Developer: Achilles 
*
* Wireframe, Build Buttons and Object Definition Files (ODFs):
*     - Activision and Mad Doc Software
*     -	Pepperman
*
* Other textures:
*    -  Activision and Mad Doc Software
*    -  Romulan disruptor textures by Rake
*	Homepage: http://www.strategyplanet.com/starmada/weapons
*       Contact: rake@strategyplanet.com
*
* Audio Files:
*     -  Activision and Mad Doc Software
*
*****************************************************************************************************

Introduction:

The Shrike class is a favorite of the Tal Shiar, the Romulan Intelligence Agency, 
for its stealth and speed. It is outfitted with a cloaking device,allowing Tal Shiar 
operatives to obtain order of battle information from the enemy. Shrike 
class vessels are equipped with two forward firing plasma cannons.
and a micro torpedo launcher.

Setup Instructions:
==========================================================================
1.  Download file
==========================================================================

Download file, virus check and extract files to a known location other than
the Armada directory

==========================================================================
2. Copy files
==========================================================================

Copy the *.SOD to your Armada SOD Directory
Copy the *.odf to your respective Armada ODF Directory
Copy the *.tga to your Armada Textures/Rgb Directory
Copy the *.bmp to your Armada bitmaps\AdmiralsLog\ShipImages Directory

==========================================================================
3. Mod the ship files and make it buildable by the construction ship
==========================================================================

Open the Romulan shipyard odf file (e.g., ryard.odf) and insert a new builditem 
under the construction parameters:

// Construction Parameters
buildItemX = "rshrike"

Where X is the next available number in the sequence.

==========================================================================
4. Mod the appropriate Techfile files
==========================================================================

Open an appropriate techtree file (e.g., tech1.tt is for standard tech 
mode) and add the following lines.  

rshrike.odf  1 ryard.odf                            // destroyer (shrike class)

==========================================================================
5. Mod the Gui_global.spr to add build buttons and wireframes
==========================================================================

Open the gui_global.spr file located in the Star Trek - Armada\Sprites
folder.

Add the following buttons under the # Romulan build buttons header:

@reference=64

# Build button for the Romualn Shrike Destroyer
b_rshrike	gbrshrike	0	0	64	64


Now add the wireframe references under the follwing header:

#Romulan Wireframes
@reference=256

# Wireframe for the Romualn Shrike Destroyer
rshrikew1	romwireframe02	0	0	48	48		
rshrikew2	romwireframe02	48	0	48	48		
rshrikew3	romwireframe02	96	0	48	48		
rshrikew4	romwireframe02	144	0	48	48		
rshrikew5	romwireframe02	192	0	48	48

==========================================================================
6. Mod the weapon.spr to add weapon references
==========================================================================

Open the weapon.spr file located in the Star Trek - Armada\Sprites
folder.

Add the following lines under the respective headers:

@reference=256
@tmaterial=additive

# Romulan Pulse Cannon
rpulse	rccdrt	28	64	175	64

@reference=128
@tmaterial=additive

==========================================================================
7. Mod the events.odf to add sound references
==========================================================================

None required.  Uses stock sounds.

==========================================================================
8. Have fun with the Romualn Shrike Destroyer
==========================================================================

I hope you enjoy this addition to ST Armada.  Have fun.

==========================================================================
9. Contact Info
==========================================================================

Feel free to drop me a line and let me know what you thought of the addon.

pepperman35@hotmail.com

==========================================================================
10. Uninstall Info
==========================================================================

Reverse the steps above to remove this ship.

==========================================================================
11. Permissions
==========================================================================
Achilles has hereby granted permission to those who wish to use this ship
in their mods providing proper credits are given.

==========================================================================
12. Legal
==========================================================================

This material is not made or supported by Activision or MAD DOC Software. This material 
is freeware and may not be use for commercial purposes!  By installing this addon, you 
(the user) agree to and assume all risks of said addon.  As a result, I take no
responsibility for any damages that may occur to your game, mod or hardware.

Star Trek and related marks are trademarks of Paramount Pictures. Activision is a 
registered trademark of Activision, Inc.  All right reserved.  All other trademarks
and trade names are the properties of their respective owners.