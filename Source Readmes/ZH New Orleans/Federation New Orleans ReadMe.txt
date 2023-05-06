
##################################################

--------------------------------------------------
Star Trek: Armada II - Zero Hour
--------------------------------------------------
Federation New Orleans Class Tactical Cruiser
--------------------------------------------------

##################################################

-------------------------
Description
-------------------------

Having proved her worth on multiple occasions, these vessels have become known as the smaller sister to both the Galaxy and Nebula respectively. Many vessels of this type played an assorted role in the multiple border confrontations throughout 2347 and 2355.

##################################################

-------------------------
Credits ~ Specifically for Ambassador
-------------------------

	- Mesh rebuilds by Aad Moreman, originals by Cpt. LC Amaral
	- Textures are credited to Cpt. LC Amaral

	Build Button, Wireframe, Admirals Log and .odf credited to Ash Stephens.
	- Alterations to meshes and textures also undertaken by me.
	- Contact: ash87uk@sky.com

##################################################

-------------------------
Credits ~ Specifically for New Orleans
-------------------------

	- Original Mesh and Textures are credited to Cpt. LC Amaral
	- Poly Reduction of Mesh undertaken by me (Ash Stephens).
	- Also replaced nacelles (see details).

	Build Button, Wireframe, Admirals Log and .odf credited to Ash Stephens.
	- Alterations to meshes and textures also undertaken by me.
	- Contact: ash87uk@sky.com

-------------------------
Details
-------------------------

Due to not liking the common kitbash, I decided to replace the nacelles on this New Orleans and give it something that didn't look like an exact replica of the Galaxy nacelle. Thus, I borrowed the nacelles from the common Dawnstar model (credited to Luan "Redragon" Ngo) and stuck them on instead.

##################################################

-------------------------
Install
-------------------------
Unless you have already modofied your Armada II Install, you wont need to overwrite anything.
-------------------------

Open the SOD folder -->

Put the sod files into the sod folder of Armada II.

Open the ODF folder -->

Put the ODF files into the odf/ships folder of Armada II.

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

b_fexplore03 gbFZHorleans 0 0 64 64


Next, scroll down and locate:

-----
#Federation wireframes
@reference=256
-----

Below, enter the following:

fexplore03w1 zhOrlWF 0 0 128 128
fexplore03w2 zhOrlWF 0 0 128 128
fexplore03w3 zhOrlWF 0 0 128 128
fexplore03w4 zhOrlWF 0 0 128 128
fexplore03w5 zhOrlWF 0 0 128 128

Save and Exit.


Open the techtree folder -->

Find 'tech1.tt' and add the following under the federation ships:

-----
fexplore03.odf 2 fupgrade.odf fyard.odf // exploration ship
-----

Next, locate the 'fulltech.tt' file, and add the following again under the federation ships:

-----
fexplore03.odf 0
-----

Save and Exit.

-----
File is now ready for skirmish use.
-----

##################################################

-------------------------
Usage Policy
-------------------------

These files are sanctioned for reuse in other Armada II Modifications through free distribution. Such the distributor need not contact me directly, though they will at all times, without excuse include this complete ReadMe in such a re-released file / completion project.

Unless specifically stated, these files are solely for Armada II use, and will not be converted to any other game, or for any other use without express permission. Conversion of these files is authorised only after acknowledgement by me.

Unless otherwise stated, these files are exclusive to FileFront, and should not be hosted elsewhere.

##################################################