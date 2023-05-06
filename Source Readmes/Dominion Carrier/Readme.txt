Dominion Carrier from Dominion Wars Class for ST:Armada 2 by Wrath of Achilles & STGamer2002

This is the Dominion Carrier as seen in the Dominion wars games, I personally don't like the design but I've had enough requests that this thing should just be done. I've armed it will with multi-targeting phasers, it should match up to four battleships.


Installation**

Move all folders (Textures, odf, SOD, bitmaps) to your Star trek armada 2 directory

Open gui_global.SPR in your sprites directory and scroll down to the cardassian build 
buttons. Add this line amongst the ships.

b_dcarrier			gbdcarrier		0	0	64	64

Then in the wireframe section at the bottom add these lines.

dcarrierw1			dccwireframe	0	0	256	256
dcarrierw2			dccwireframe	0	0	256	256
dcarrierw3			dccwireframe	0	0	256	256
dcarrierw4			dccwireframe	0	0	256	256
dcarrierw5			dccwireframe	0	0	256	256

Open tech1.TT in your techtree folder and add this line.
(for neatness sake you can place with other Cardassian listings)

dcarrier.odf  2 cyard2.odf cresear2.odf

Open cyard2.odf in your odf/stations directory and scroll down to the build list and add 
this after buildItem7

buildItem4 = "dcarrier"

or, to put it in it's correct place alter the list so this ship is under the ccruise1.
remember to keep the build list in ascending sequence.

All is done, enjoy.


Additional Information**

at 1496 polies this ship is fine for a heavy battleship/dreadnought and should not present any problems for low end machine users.

The sod and textures will work not work in armada 1, Email me for help on this
if needed.

Feel free to use this in any mod so long as credit is given to me for the model
and textures and STGamer2002 for button, odf and borg textures.

Feel free to edit the odfs in any way so long as credit is given, please contact me
if you wish to alter the model or textures.



Legal Stuff**

The material submitted with this readme is in no way connected to, or affiliated 
with Activision, its employees, representatives, consortiums, or other bodies 
directly or indirectly associated with the afore mentioned company. Therefore 
if the files contained in this mod cause damage to your system in any way then 
Activision cannot be held responsible or liable.

USE AT YOUR OWN RISK.



Credits**

Thanks to STGamer2002 who helped me with the entire release.



Contact**

Thanks, achilles
wrathofachilles@hotmail.com

STGamer2002
zorgus@hotmail.com
