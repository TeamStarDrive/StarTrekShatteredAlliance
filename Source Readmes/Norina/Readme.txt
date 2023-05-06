Cardassian Norin Class for ST:Armada 2 by Wrath of Achilles

This is the Norin class originally shown in the Star Trek game "The Dominion Wars",
The mesh and texture has been completely scrath built by me from reference shots
and I'm aware it's not exact, I never like them to be ;). I've designated this a very
heavy destroyer, sort of a notch down from the brinok ingame.


Installation**

Move all folders (Textures, odf, SOD, bitmaps) to your Star trek armada 2 directory

Open gui_global.SPR in your sprites directory and scroll down to the cardassian build 
buttons. Add this line amongst the ships.

b_cdestroy3			gbcdestroy3		0	0	64	64

Then in the wireframe section at the bottom add these lines.

cdestroy3w1			cd3wireframe	0	0	48	48
cdestroy3w2			cd3wireframe	48	0	48	48
cdestroy3w3			cd3wireframe	96	0	48	48
cdestroy3w4			cd3wireframe	144	0	48	48
cdestroy3w5			cd3wireframe	192	0	48	48

Open tech1.TT in your techtree folder and add this line.
(for neatness sake you can place with other Cardassian listings)

cdestroy3.odf 1 cyard.odf 

Open cyard.odf in your odf/stations directory and scroll down to the build list and add 
this after buildItem7

buildItem8 = "cdestroy3"

or, to put it in it's correct place alter the list so this ship is under the ccruise1.
remember to keep the build list in ascending sequence.

All is done, enjoy.


Additional Information**

at 1026 polies and one texture you should be fine mass producing this ship ingame.

The sod and textures will work not work in armada 1, Email me for help on this
if needed.

Feel free to use this in any mod so long as credit is given to me for the model
and textures.

Feel free to edit the odfs in any way so long as credit is given, please contact me
if you wish to alter the model or texture.



Legal Stuff**

The material submitted with this readme is in no way connected to, or affiliated 
with Activision, its employees, representatives, consortiums, or other bodies 
directly or indirectly associated with the afore mentioned company. Therefore 
if the files contained in this mod cause damage to your system in any way then 
Activision cannot be held responsible or liable.

USE AT YOUR OWN RISK.



Credits**

Thanks to Major A Payne for reminding me to make this model.

Thanks to STGamer2002 who is helping me out with some mod stuff :)

Thanks to who ever sent in some reference shots, I dont remember the name, sorry.



Contact**

Thanks, achilles

wrathofachilles@hotmail.com