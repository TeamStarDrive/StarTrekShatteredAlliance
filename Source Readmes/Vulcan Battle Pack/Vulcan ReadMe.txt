
##################################################

--------------------------------------------------
Star Trek: Armada II - Zero Hour
--------------------------------------------------
Drelex Class Assault Ship
Sotek Class Heavy Cruiser
Tokra Class Warship
--------------------------------------------------
Vulcan Naval Shipyard (Inc)
--------------------------------------------------

##################################################

Drelex: Generally thought of as an interceptor, these small Vulcan vessels are typically used as scouts, or to support the larger Sotek. Roughly the size of the Federation Sabre, the Drelex type, whilst not very powerful are fairly quick on their feet, usually able to avoid slow moving weaponry.

Sotek: The flame that drives Vulcan Logic. Almost rivalling a Klingon Vor’cha in size, the Sotek are considerably well armoured for a Vulcan Vessel. In addition to their size, these large red vessels can provide, as well as receive quite a pounding from enemy fire.

Tokra: Rivalling the Federation Galaxy in size, the Tok'ra is a formidable Warship of the Vulcan Navy. Looking in the way of the Romulan Warbird's sheer mass, the Tok'ra is used to justify a stance by the Vulcan independence shortly after the separation from the Federation.

##################################################

-------------------------
Credits
-------------------------

	- Mesh and Textures credited to Aad Moreman 
	- Concept for the Drelex and Sotek are via Altom
	- Concept for the Tokra and Vulcan Shipyard via Aad Moreman

	- Wireframe, Build Button, AdmiralsLog Image, and other game-files were compiled by me (Ash Stephens).
	- Contact: ash87uk@sky.com

##################################################

-------------------------
Install
-------------------------
Unless you have already modofied your Armada II Install, you wont need to overwrite anything.
-------------------------

Open the SOD folder -->

Put the sod files into the sod folder of Armada II.

Open the ODF folder -->

Put the ODF files into the odf folders of Armada II.

Open the Textures/RGB folder -->

Put the TGA files into the Textures/RGB folder of Armada II.

Open the Bitmaps folder -->

Put the BMP files into the Bitmaps/AdmiralsLog/ShipImages folder of Armada II.


Open the Sprites folder -->

Find the 'gui_global.spr' file and open it.
Scroll down and locate:

-----
# Federation build buttons
@reference=64
@tmaterial=default
-----

Below the 'b_fspecial' line, add the following:

b_NAVcombat01 	gbZHdrelex		0 0 64 64
b_NAVcombat02 	gbZHsotek		0 0 64 64
b_NAVcombat03 	gbZHtokra		0 0 64 64
b_npcNAVyard	gbZHvulyard 		0 0 64 64

Next, scroll down and locate:

-----
#Federation wireframes
@reference=256
-----

Below, enter the following:

NAVcombat01w1 	zhVulWF 		0 0 128 128
NAVcombat01w2 	zhVulWF 		0 0 128 128
NAVcombat01w3 	zhVulWF 		0 0 128 128
NAVcombat01w4 	zhVulWF 		0 0 128 128
NAVcombat01w5 	zhVulWF 		0 0 128 128

NAVcombat02w1 	zhVulWF 		128 256 128 128
NAVcombat02w2 	zhVulWF 		128 256 128 128
NAVcombat02w3 	zhVulWF 		128 256 128 128
NAVcombat02w4 	zhVulWF 		128 256 128 128
NAVcombat02w5 	zhVulWF 		128 256 128 128

NAVcombat03w1 	zhVulWF 		256 128 128 128
NAVcombat03w2 	zhVulWF 		256 128 128 128
NAVcombat03w3 	zhVulWF 		256 128 128 128
NAVcombat03w4 	zhVulWF 		256 128 128 128
NAVcombat03w5 	zhVulWF 		256 128 128 128

npcNAVyardw1 	zhVulWF			128 128 128 128
npcNAVyardw2 	zhVulWF 		128 128 128 128
npcNAVyardw3 	zhVulWF 		128 128 128 128
npcNAVyardw4 	zhVulWF 		128 128 128 128
npcNAVyardw5 	zhVulWF 		128 128 128 128

Save and Exit.


Open the techtree folder -->

Find 'tech1.tt' and add the following under the federation ships:

-----
NAVcombat01.odf	0	// assault ship
NAVcombat02.odf	0	// cruiser
NAVcombat03.odf	0	// warship
npcNAVyard.odf	0	// shipyard
-----

Next, locate the 'fulltech.tt' file, and add the following again under the federation ships:

-----
NAVcombat01.odf	0
NAVcombat02.odf	0
NAVcombat03.odf	0
npcNAVyard.odf	0
-----

Save and Exit.

-----
File is now ready for skirmish use.

##################################################

-------------------------
Usage Policy
-------------------------

These files are sanctioned for reuse in other Armada II Modifications through free distribution. Such the distributor need not contact me directly, though they will at all times, without excuse include this complete ReadMe in such a re-released file / completion project.

Unless specifically stated, these files are solely for Armada II use, and will not be converted to any other game, or for any other use without express permission. Conversion of these files is authorised only after acknowledgement by me.

Unless otherwise stated, these files are exclusive to Armada2Files (FileFront Network) and MSFC (Majestic Sci-Fi Central), and should not be hosted elsewhere.

##################################################