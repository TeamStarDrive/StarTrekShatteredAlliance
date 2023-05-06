*******************************************************************************************
* Model Credits:
*  Tal Shiar Warbird v.1.0
*    -  Game: Star Trek Armada
*    -	Mesh Developer: Atrahasis
*    -	Texture Developer: Atrahsis
*    -  Conversion from SFC and other modifications by Pepperman
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
*    -  Romulan phaser beam and photon torpedo by Activision and Mad Doc Software
*
* Audio Files:
*     -  Activision and Mad Doc Software
*
* Special Thanks to Armada Fleet Command (AFC) for their great site :)
*****************************************************************************************************

Introduction:

The N'Neikha Class is a Tal Shiar Warbird designed for combat operations.  It
is equipped with Shield Inversion beam, phasers, disruptors and photon torpedoes.
It, like all other ships in the Romulan fleet, has the standard cloaking device.

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
Copy the *.odf to your Armada Addon Directory
Copy the *.wav to your Armada Addon Directory
Copy the *.tga to your Armada Textures/Rgb Directory

==========================================================================
3. Mod the ship files and make it buildable by the shipyard
==========================================================================

Open a shipyard.odf file (e.g., ryard2.odf, ryard3.odf) and insert a new builditem 
under the construction parameters:

// Construction Parameters
buildItemX = "rwarbird"

Where X is the next available number in the sequence.

==========================================================================
4. Mod the appropriate Techfile files
==========================================================================

Open an appropriate techtree file (e.g., tech1.tt is for standard tech mode)
and add the following lines:

rwarbird.odf 0

==========================================================================
5. Mod the Gui_global.spr to add build buttons and wireframes
==========================================================================

Open the gui_global.spr file located in the Star Trek - Armada\Sprites
folder.

Add the following under the appropriate # Romulan header:

# Romulan build buttons
@reference=64
b_rwarbird	gbrwarbird	0	0	64	64


# Ship Wireframes
@reference=128
@tmaterial=interface
rwarbirdw1		RWrwarbird	40	0	40	40		
rwarbirdw2		RWrwarbird	0	40	40	40		
rwarbirdw3		RWrwarbird	40	40	40	40		
rwarbirdw4		RWrwarbird	80	0	40	40		
rwarbirdw5		RWrwarbird	0	0	40	40

==========================================================================
6. Mod the weapon.spr to add weapon references
==========================================================================

Open the weapon.spr file located in the Star Trek - Armada\Sprites
folder.

Add the following lines under the respective headers:

@reference=256
@tmaterial=additive

# Tal Shiar Warbird Disruptor Cannon
rwbpulse	rwbpulse	0	0	235	80

@reference=128
@tmaterial=additive

# Tal Shiar Warbird Photon Torpedo
rwbphot		wrtorp		0	0	32	32	@anim=tex4x4

# Tal Shiar Warbird phaser
rwbphas		wrwbphas	0	0	128	32	@anim=tex1x4

==========================================================================
7. Mod the events.odf to add sound references
==========================================================================

None.  It is setup to use Sela's voice files.

###################################################################################

==========================================================================
8. Have fun with the Tal Shiar Warbird
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
11. Legal
==========================================================================

This material is not made or supported by Activision or MAD DOC Software. This material 
is freeware and may not be use for commercial purposes!  By installing this addon, you 
(the user) agree to and assume all risks of said addon.  As a result, I take no
responsibility for any damages that may occur to your game, mod or hardware.

Star Trek and related marks are trademarks of Paramount Pictures. Activision is a 
registered trademark of Activision, Inc.  All right reserved.  All other trademarks
and trade names are the properties of their respective owners.
