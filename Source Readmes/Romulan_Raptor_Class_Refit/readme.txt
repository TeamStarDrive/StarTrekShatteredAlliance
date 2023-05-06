*******************************************************************************************
* Model Credits:
*  Romulan Raptor Class Refit v1.0
*    -  Game: Star Trek Armada 1
*    -	Mesh Developer: Activision and Mad Doc Software
*    -	Texture Developer: Activision and Mad Doc Software
*    -  Additiional modifications by Pepperman 
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
*
* Audio Files:
*     -  Activision and Mad Doc Software
*
* Special thanks to Armada Fleet Command (AFC) for supporting the
* Star Trek Gaming Community
*****************************************************************************************************

Introduction:

The Romulan Raptor Class Torpedo Cruiser has been refitted with new warp 
engines, medium disruptors for defense and dual torpedo launchers that fire 
the modified version of the Federation's tri-cobalt torpedoes.  These 
torpedoes are very effective as long-range artillery and can cause tremendous 
damage. All refitted Raptors can be equipped with a Myotronic Inhibitor 
torpedo which temporarily disables the weapons system of an enemy vessel, 
rendering them ineffective in combat.


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

Open the Romulan shipyard odf file (e.g., ryard.odf) and insert a new builditem 
under the construction parameters:

// Construction Parameters
buildItemX = "rraptor"

Where X is the next available number in the sequence.

==========================================================================
4. Mod the appropriate Techfile files
==========================================================================

Open an appropriate techtree file (e.g., tech1.tt is for standard tech mode)
and add the following lines. 

rraptor.odf  1 rresear.odf

==========================================================================
5. Mod the Gui_global.spr to add build buttons and wireframes
==========================================================================

Open the gui_global.spr file located in the Star Trek - Armada\Sprites
folder.

Add the following buttons under the # Romulan build buttons header:

@reference=64

# Build button for the Romulan Raptor Class Refit
b_rraptor	gbrraptor	0	0	64	64

Now add the wireframe references under the follwing header:

# Building Wireframes
@reference=128

# Wireframe for the Raptor Class Refit
rraptorw1		rwcrus2		40	0	40	40		
rraptorw2		rwcrus2		0	40	40	40		
rraptorw3		rwcrus2		40	40	40	40		
rraptorw4		rwcrus2		80	0	40	40		
rraptorw5		rwcrus2		0	0	40	40		
	
==========================================================================
6. Mod the weapon.spr to add weapon references
==========================================================================

Open the weapon.spr file located in the Star Trek - Armada\Sprites
folder.

Add the following lines under the respective headers:

@reference=256
@tmaterial=additive

# Romulan Medium Disruptor Cannon for the Raptor Class Refit
rrtdptm		rccdrt		0	0	235	80

@reference=128
@tmaterial=additive

# Romulan Modified Tri-Cobalt Torpedoes
spphoton	spphoton	0	0	32	32	@anim=tex4x4

==========================================================================
7. Mod the events.odf to add sound references
==========================================================================

Open the events.odf file located in the main Armada directory and add the following lines.

#################################################################################
# Cruiser6 SOUNDS

Cruiser6Acknowledge{
Table
	Sound <borg> "gvobor30.wav"
	Sound <federation> "gvofc101.wav"
	Sound <klingon> "gvokc101.wav"
	Sound <romulan> "rrap101.wav"
}

Cruiser6Select{
Table
	Sound <borg> "gvobor17.wav"
	Sound <borg> "gvobor19.wav"
	Sound <borg> "gvobor60.wav"
	Sound <federation> "gvofc116.wav"
	Sound <federation> "gvofc117.wav"
	Sound <federation> "gvofc118.wav"
	Sound <klingon> "gvokc116.wav"
	Sound <klingon> "gvokc117.wav"
	Sound <klingon> "gvokc118.wav"
	Sound <romulan> "rrap216.wav"
	Sound <romulan> "rrap217.wav"
	Sound <romulan> "rrap218.wav"
}

Cruiser6Attack{
Table
	Sound <borg> "gvobor06.wav"
	Sound <borg> "gvobor09.wav"
	Sound <borg> "gvobor42.wav"
	Sound <federation> "gvofc106.wav"
	Sound <federation> "gvofc107.wav"
	Sound <federation> "gvofc108.wav"
	Sound <klingon> "gvokc106.wav"
	Sound <klingon> "gvokc107.wav"
	Sound <klingon> "gvokc108.wav"
	Sound <romulan> "rrap206.wav"
	Sound <romulan> "rrap207.wav"
	Sound <romulan> "rrap208.wav"
	Sound <borg> "gvobor30.wav"
	Sound <klingon> "gvokc101.wav"
	Sound <romulan> "rrap201.wav"
	Sound <borg> "gvobor19.wav"
	Sound <borg> "gvobor60.wav"
	Sound <federation> "gvofc116.wav"
	Sound <federation> "gvofc117.wav"
	Sound <klingon> "gvokc117.wav"
	Sound <klingon> "gvokc118.wav"
	Sound <romulan> "rrap216.wav"
	Sound <romulan> "rrap217.wav"
}

Cruiser6Stop{
Table
	Sound <borg> "gvobor23.wav"
	Sound <federation> "gvofc121.wav"
	Sound <klingon> "gvokc121.wav"
	Sound <romulan> "rrap221.wav"
}

Cruiser6Move{
Table
	Sound <borg> "gvobor11.wav"
	Sound <borg> "gvobor12.wav"
	Sound <borg> "gvobor13.wav"
	Sound <borg> "gvobor14.wav"
	Sound <federation> "gvofc111.wav"
	Sound <federation> "gvofc112.wav"
	Sound <federation> "gvofc113.wav"
	Sound <klingon> "gvokc111.wav"
	Sound <klingon> "gvokc112.wav"
	Sound <klingon> "gvokc113.wav"
	Sound <romulan> "rrap211.wav"
	Sound <romulan> "rrap212.wav"
	Sound <romulan> "rrap213.wav"
	Sound <borg> "gvobor30.wav"
	Sound <klingon> "gvokc101.wav"
	Sound <romulan> "rrap201.wav"
	Sound <borg> "gvobor19.wav"
	Sound <borg> "gvobor60.wav"
	Sound <federation> "gvofc116.wav"
	Sound <federation> "gvofc117.wav"
	Sound <klingon> "gvokc117.wav"
	Sound <klingon> "gvokc118.wav"
	Sound <romulan> "rrap216.wav"
	Sound <romulan> "rrap217.wav"
}
	
Cruiser6Repair{
Table
	Sound <borg> "gvobor26.wav"
	Sound <federation> "gvofc126.wav"
	Sound <klingon> "gvokc126.wav"
	Sound <romulan> "rrap226.wav"
}

###################################################################################


==========================================================================
8. Have fun with the Romulan Raptor Class Refit
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