*******************************************************************************************
* Name: KDF C-9 “Warblood” (ghob ‘lw) Class Battleship
*
* Version: 1.0
*
* Game: Armada II
*
* Model Credits:
*    -  Game: Star Trek Armada II
*    -  Ship Design: Raven Night
*    -	Mesh Developer: Raven Night
*         + RavenNight@Hotmail.com
*         + See original read me file (C9 Readme.doc)
*    -	Texture Developer: Raven Night
*    -  Conversion By: Pepperman 
*
* Wireframe, Build Buttons and Object Definition Files (ODFs):
*     - Activision and Mad Doc Software
*     -	Pepperman
*
* Other textures:
*    -  Activision and Mad Doc Software
*    -  Klingon pulse and torpedo textures by Rake
*	  + Homepage: http://www.strategyplanet.com/starmada/weapons
*         + Contact: rake@strategyplanet.com
*    -  EMP beam textures by AnunC8 (Unique Weapon Sprites (Modder's Resource)
*         + Contact: anunc8(@)yahoo(.)com
*
* Audio Files:
*     -  None.  Uses stock sounds.
*
* Permissions:  See original read me file (C9 Readme.doc)
*
* Notes: This release is a high poly count version.  The model (8,462 plys)
* incudes two high definition texture maps (2048 x 2048). 
* 
*****************************************************************************************************
Introduction

The Klingon Defense Force C-9 Warblood class battleship was put into service 
in approximately 2360.  The ship is reported to be in the same class range as 
the Neghvar, though classified as a battleship due to its lighter shielding 
and armor.  She is equipped with weaponry equivalent to the Neghvar; however, 
the Warblood boasts an experimental Electromagnetic Pulse (EMP) generator.  The 
EMP is in effect an electromagnetic shockwave.  This pulse of energy produces a 
powerful electromagnetic field, particularly within the vicinity of the weapon 
burst, which can generate short lived transient voltages (thousands of volts) 
thereby causing damage to a ship or stations electrical and electro-mechanical 
equipment.


Setup Instructions:
==========================================================================
1.  Download file
==========================================================================

Download file, virus check and extract files to a known location other than
the Armada II directory

==========================================================================
2. Copy files
==========================================================================

Copy the *.SOD to your SOD Directory
  C:\Program Files\Activision\Star Trek Armada II\SOD

Copy the *.odf to your Odf Directories
  C:\Program Files\Activision\Star Trek Armada II\odf\ships
  C:\Program Files\Activision\Star Trek Armada II\odf\special_weapons
  C:\Program Files\Activision\Star Trek Armada II\odf\weapons

Copy the *.tga to your Textures/Rgb Directory
  C:\Program Files\Activision\Star Trek Armada II\Textures\RGB

Copy the *.bmp to your bitmaps directory
  C:\Program Files\Activision\Star Trek Armada II\bitmaps\AdmiralsLog\ShipImages

==========================================================================
3. Mod the ship files and make it buildable by the shipyard
==========================================================================

Open the Federation shipyard odf file (e.g., kyard2.odf) and insert a 
new builditem under the construction parameters:

// Construction Parameters
buildItemX = "kblood"

Where X is the next available number in the sequence.

==========================================================================
4. Mod the appropriate Techfile files
==========================================================================

Open an appropriate techtree file (e.g., tech1.tt is for standard tech mode)
and add the following lines.  

kblood.odf      1  kyard2.odf
gkbldcloak.odf  0
gempwpn.odf     0

==========================================================================
5. Mod the Gui_global.spr to add build buttons and wireframes
==========================================================================

Open the gui_global.spr file located in the Sprites
folder.  

  C:\Program Files\Activision\Star Trek Armada II\Sprites

Add the following lines under the # Klingon build buttons header:

@reference=64

b_kblood			gbkblood		0	0	64	64
b_gkbldcloak			gkbldcloak		0	0	64	64
b_gempwpn			gbempwpn		0	0	64	64

Now add the wireframe references under the follwing header:

# Klingon wireframes
@reference=256

# Wireframe for the “Warblood” Class Battleship 

kbloodw1			kbloodwireframe		0	0	48	48	
kbloodw2			kbloodwireframe		48	0	48	48	
kbloodw3			kbloodwireframe		96	0	48	48	
kbloodw4			kbloodwireframe		144	0	48	48	
kbloodw5			kbloodwireframe		192	0	48	48

==========================================================================
6. Mod the weapon.spr to add weapon references
==========================================================================

Open the weapon.spr file located in the Sprites
folder.

  C:\Program Files\Activision\Star Trek Armada II\Sprites

Add the following lines under the respective headers:

@reference=512
@tmaterial=additive

# EMP transportor beam
empbeam		empbeam		0	0	512	128	@anim=tex1x4      


@reference=256
@tmaterial=additive

# Klingon disruptor cannons
wkpulse2	wkpulse2	32	32	192	160

# Klingon Type 7 Torpedo launcher
wktorp2		wktorp2		0	0	85	85	@anim=tex3x3

@reference=128
@tmaterial=additive

# Heavy disruptor cannons
wkpulse1	wnpulse1	3	3	64	64

# Klingon Defensive pulse disruptors
wkpulse3	wkpulse3	9	0	118	83

empwpn		empgen2		0	64	128	32

==========================================================================
7. Mod the damage.spr to add/upgrade damage mechanisms
==========================================================================

Open the damage.spr located in the Sprites folder.

  C:\Program Files\Activision\Star Trek Armada II\Sprites

Add the following lines:

@reference=128
@tmaterial=additive
origin		xspark01		0	0	32	32	@anim=tex4x4

==========================================================================
8. Have fun with the KDF C-9 “Warblood”
==========================================================================

I hope you enjoy this addition to ST Armada II.  Have fun.

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
11. Legal
==========================================================================

This material is not made or supported by Activision or MAD DOC Software. This material 
is freeware and may not be use for commercial purposes!  By installing this addon, you 
(the user) agree to and assume all risks of said addon.  As a result, I take no
responsibility for any damages that may occur to your game, mod or hardware.

Star Trek and related marks are trademarks of Paramount Pictures. Activision is a 
registered trademark of Activision, Inc.  All right reserved.  All other trademarks
and trade names are the properties of their respective owners.
