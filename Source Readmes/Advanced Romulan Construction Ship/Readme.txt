*******************************************************************************************
* Model Credits:
*  Advanced Romualn Construction Ship v.1.0
*    -  Game: Star Trek Armada
*    -	Mesh Developer: Taldren, Activision and Mad Doc Software
*    -	Texture Developer: Taldren, Activision, Mad Doc Software
*       and Atrahsis' Warbird Textures which were orginally applied
*       by Klingon Fanatic
*    -  Additiional modifications by Pepperman
     -  Note: This is a conversion from SFC
*
*  Tal Shiar Advacned Shipyard
*    -	Mesh Developer: Activision and Mad Doc Software
*    -	Texture Developer: Activision and Mad Doc Software
*    -  Additiional modifications to texture by Pepperman
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
* Special Thanks to Armada Fleet Command (AFC)
*****************************************************************************************************

Introduction:

The advanced Romulan construction ship has been designed to build all 
of the Star Empire's most advanced facilities.  Equipped with the standard 
Romulan cloaking device, the advanced construction ship can travel to nearby
quadrants undetected and establish a Romulan foothold within that sector.  
Unlike the standard construction vessel, the advanced model comes armed 
with disruptor cannons, and multiple targeting myotron inhibitor torpedoes 
in order to defend itself during its highly sensitive missions.

One of the advanced facilities that can be constructed is the Tal Shiar
advanced shipyard.  The Tal Shiar advanced shipyard serves as a focal point 
for the Tal Shiar's shipbuilding endeavors.  The advanced shipyard can build 
the Shadow, D'deridex, and the Scimitar class vessels (assuming that you have
downloaded my Scimitar mod). Because of the clandestine methods used to 
acquire the shipyard's blueprints from the Dominion, the Tal Shiar have 
classified its very existence as TOP SECRET.

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
3. Mod the ship files and make it buildable by the Romulan starbase
==========================================================================

Open the Romulan Starbase odf file (e.g., rbase.odf) and insert a new builditem 
under the construction parameters:

// Construction Parameters
buildItemX = "rconst2"

Where X is the next available number in the sequence.

==========================================================================
4. Mod the appropriate Techfile files
==========================================================================

Open an appropriate techtree file (e.g., tech1.tt is for standard tech mode)
and add the following lines.  Notice that you cannot build the advanced
construction vessel unless you have previously constructed the standard 
Romulan Starbase and advanced shipyard.

rconst2.odf  2 rbase.odf ryard2.odf
ryard3.odf   2 rbase.odf ryard2.odf

==========================================================================
5. Mod the Gui_global.spr to add build buttons and wireframes
==========================================================================

Open the gui_global.spr file located in the Star Trek - Armada\Sprites
folder.

Add the following buttons under the # Romulan build buttons header:

@reference=64

# Build button for the Advanced Romulan Construction Ship
b_rconst2	gbrconst2	0	0	64	64

# Build button for the Tal Shiar Advanced Shipyard
b_ryard3	gbryard3	0	0	64	64

Now add the wireframe references under the follwing header:

# Building Wireframes
@reference=128

# Wireframe for the Advanced Romulan Construction Ship
rconst2w1	RWrconst2	40	0	40	40
rconst2w2	RWrconst2	0	40	40	40
rconst2w3	RWrconst2	40	40	40	40
rconst2w4	RWrconst2	80	0	40	40
rconst2w5	RWrconst2	0	0	40	40

# Wireframe for the Tal Shiar Advanced Shipyard
ryard3w1	jwyard		40	0	40	40		
ryard3w2	jwyard		0	40	40	40		
ryard3w3	jwyard		40	40	40	40		
ryard3w4	jwyard		80	0	40	40		
ryard3w5	jwyard		0	0	40	40	

==========================================================================
6. Mod the weapon.spr to add weapon references
==========================================================================

Open the weapon.spr file located in the Star Trek - Armada\Sprites
folder.

Add the following lines under the respective headers:

@reference=256
@tmaterial=additive

# Advanced Construction Ship (Romulan) Disruptor Cannon
rfdispt		rfdispt		0	0	235	80

==========================================================================
7. Mod the events.odf to add sound references
==========================================================================

#################################################################################
# Advanced Construction ship SOUNDS

AdvConstructAcknowledge{
Table
	Sound <borg> "gvobor34.wav"
	Sound <borg> "gvobor05.wav"
	Sound <borg> "gvobor32.wav"
	Sound <federation> "gvofcc01.wav"
	Sound <federation> "gvofcc02.wav"
	Sound <federation> "gvofcc03.wav"
	Sound <klingon> "gvokcc01.wav"
	Sound <klingon> "gvokcc02.wav"
	Sound <klingon> "gvokcc03.wav"
	Sound <romulan> "gvorcc90.wav"
	Sound <romulan> "gvorcc91.wav"
	Sound <romulan> "gvorcc92.wav"
}

AdvConstructSelect{
Table
	Sound <borg> "gvobor17.wav"
	Sound <borg> "gvobor61.wav"
	Sound <borg> "gvobor18.wav"
	Sound <federation> "gvofcc16.wav"
	Sound <federation> "gvofcc17.wav"
	Sound <federation> "gvofcc18.wav"
	Sound <klingon> "gvokcc16.wav"
	Sound <klingon> "gvokcc17.wav"
	Sound <klingon> "gvokcc18.wav"
	Sound <romulan> "gvorcc96.wav"
	Sound <romulan> "gvorcc97.wav"
	Sound <romulan> "gvorcc98.wav"
}

AdvConstructStop{
Table
	Sound <borg> "gvobor22.wav"
	Sound <federation> "gvofcc21.wav"
	Sound <klingon> "gvokcc21.wav"
	Sound <romulan> "gvorcc99.wav"
}

AdvConstructMove{
Table
	Sound <borg> "gvobor11.wav"
	Sound <borg> "gvobor12.wav"
	Sound <borg> "gvobor13.wav"
	Sound <borg> "gvobor14.wav"
	Sound <federation> "gvofcc11.wav"
	Sound <federation> "gvofcc12.wav"
	Sound <federation> "gvofcc13.wav"
	Sound <klingon> "gvokcc11.wav"
	Sound <klingon> "gvokcc12.wav"
	Sound <klingon> "gvokcc13.wav"
	Sound <romulan> "gvorcc93.wav"
	Sound <romulan> "gvorcc94.wav"
	Sound <romulan> "gvorcc95.wav"
	Sound <borg> "gvobor34.wav"
	Sound <borg> "gvobor05.wav"
	Sound <borg> "gvobor32.wav"
	Sound <federation> "gvofcc01.wav"
	Sound <federation> "gvofcc02.wav"
	Sound <klingon> "gvokcc01.wav"
	Sound <klingon> "gvokcc02.wav"
	Sound <klingon> "gvokcc03.wav"
	Sound <romulan> "gvorcc90.wav"
	Sound <romulan> "gvorcc91.wav"
	Sound <romulan> "gvorcc92.wav"
}
	
AdvConstructRepair{
Table
	Sound <borg> "gvobor26.wav"
	Sound <federation> "gvofcc26.wav"
	Sound <klingon> "gvokcc26.wav"
	Sound <romulan> "gvorcc89.wav"
}


###################################################################################


###################################################################################

==========================================================================
8. Have fun with the Advanced Romualn Construction Ship!
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