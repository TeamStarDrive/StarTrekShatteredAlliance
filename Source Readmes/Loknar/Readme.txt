Cardassian Loknar Class Heavy cruiser Ship by Wrath of Achilles

This is my own design, It was roughly designed around the federation
steamrunner. I made two versions of the sod, 1 with a canon and 1
with a weapons pod. the weapons pod version functions as a heavy cruiser
and the canon one is an artillery ship. You can only build the heavy cruiser 
version and this can refit in space to the artillery version and back again.


Installation**

Move all folders (Textures, odf, SOD) to your Star trek armada 2 directory

Open gui_global.SPR and scroll down to the cardassian build buttons.
add this line over the old ccolony button reference.

b_cloknara			gbloknar		0	0	64	64

Further down to the special weapons build buttons add these lines

b_gloknar1			gloknar1		0	0	64	64
b_gloknar2			gloknar2		0	0	64	64

Open tech1.TT and add this line over the existing ccolony listing
(for neatness sake you can place with other Cardassian listings)

cloknara.odf 2 cyard.odf cresear.odf
gloknar1.odf 0
gloknar2.odf 0 

Open cyard.odf and scroll down to the build list and add this after buildItem7

buildItem8 = "cloknara"



Additional Information**

The sod and textures will work in armada 1, file order will have to be changed
for the odfs and they will need editing quite a lot, Email me for help on this
if needed.

Feel free to use this in any mod so long as credit is given to me for the model
and textures, you can use either version of the ship.

Feel free to edit the textures/model/odfs in any way so long as credit is given.

Apologies for having no wireframes, STGamer2002 normally does them for
me but he's off modding atm ;)



Legal Stuff**

The material submitted with this readme is in no way connected to, or affiliated 
with Activision, its employees, representatives, consortiums, or other bodies 
directly or indirectly associated with the afore mentioned company. Therefore 
if the files contained in this mod cause damage to your system in any way then 
Activision cannot be held responsible or liable.

USE AT YOUR OWN RISK.



Credits**

Thanks to Major A Payne for his opinions during creation.



Contact**

Thanks, achilles

wrathofachilles@hotmail.com