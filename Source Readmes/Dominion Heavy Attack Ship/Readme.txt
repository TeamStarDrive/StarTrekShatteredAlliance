Dominion Heavy Attack Class for ST:Armada 2 by Wrath of Achilles

This is the Dominion Heavy Attack ship designed to fill the role of heavy cruiser.
Designed by Azel/Atolm and requested by Major A Payne. she is 2022 polies.
I did not want this ship to have a weapon but an increased loadout as it's supposed
to be pure aggression, the phalanx torpedos were inspired by the same weapons
on the achilles class.

I have the Dominion Carrier from DW made but it didn't come out as great as it should
I will probably release anyway as I know most people want the ship.

Installation**

Move all folders (Textures, odf, SOD, bitmaps) to your Star trek armada 2 directory

Open gui_global.SPR in your sprites directory and scroll down to the cardassian build 
buttons. Add this line amongst the ships.

b_dcruise3			gbdcruise3		0	0	64	64

Then in the wireframe section at the bottom add these lines.

dcruise3w1			dc3wireframe	0	0	48	48
dcruise3w2			dc3wireframe	48	0	48	48
dcruise3w3			dc3wireframe	96	0	48	48
dcruise3w4			dc3wireframe	144	0	48	48
dcruise3w5			dc3wireframe	192	0	48	48

Open tech1.TT in your techtree folder and add this line.
(for neatness sake you can place with other Cardassian listings)

dcruise3.odf  2 cyard.odf cresear.odf

Open cyard.odf in your odf/stations directory and scroll down to the build list and add 
this after buildItem7

buildItem8 = "dcruise3"

or, to put it in it's correct place alter the list so this ship is under the ccruise1.
remember to keep the build list in ascending sequence.

All is done, enjoy.


Additional Information**

at 2022 polies and being a cruiser there could be computer issues with low end machines
but unless you running a compaq you nicked from the office you should be ok.

The sod and textures will work not work in armada 1, Email me for help on this
if needed.

Feel free to use this in any mod so long as credit is given to me for the model
and textures, and Azel/Atolm for the Design.

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

Thanks to Major A Payne for suggesting the model and his opinions
during production and many other things.

Thanks to STGamer2002 who offered to convert for me and is going
to helping out with some mods soon I hope.



Contact**

Thanks, achilles

wrathofachilles@hotmail.com