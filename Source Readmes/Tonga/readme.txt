Cardassian Tonga class by Wrath of Achilles

This ship was designed for the dominion wars game, I didn't stick too closely to the design because
I wanted to play around with it, to that end there are 5 variants. Here are the tooltips from each version.

Standard
With the Successful Klingon blockade of Cardassia Prime, a stranglehold was put on the Cardassian war industry. All of their conveys and most of their blockade runners were being intercepted by the Klingons. In a desperate effort to break the blockade Cardassian engineers went back to a 50-year-old design that could utilize locally available raw materials.

Sensor (large scan range, detects cloaks)
Cloaking technology was allowing the Klingon Bird of Preys to attack at will with little or no defence being offered. To counteract this a large amount of the refitted Tonga class vessels had a large sensor pod and astrometrics facilities added.

Assault (lots of extra crew, assault transport mode and very strong boarding parties)
Tonga Class - Assault variant"
verboseTooltip = "Whilst gaining the upper hand in many skirmishes the Tonga captains noted they had incapacitated an enemy vessel only to have to destroy it due to lack of soldiers and transport facilities. To enable the capture of damaged vessels the Tonga has been refitted with advanced transporters and a large number of specially trained soldiers.

Weapon (Two additional phasers)
Despite the success story that was the Tonga rebirth the Cardassian captains frequently found themselves outgunned and without backup, to this end several of the Tongas were refitted with additional Beam emitters to surprise an unaware opponent.

Total (All of the above upgrades in one)
With the Tongas successfully breaking through the Klingon blockades and bringing much needed materials into Cardassian space the order has been given to add all availble refits to the remaining Tonga class ships, the result is a formidable and versatile battlleship.



Installation**

All files edited during this installation should be backed up for ease of removal. odf, tt and spr files
are all edited with notepad or wordpad just make sure they aren't marked as read only (right click on the
file to check this)

Move these folders (Textures, odf, Sod) to your Star trek armada 2 directory

Open the sprites folder then on gui_global.spr, scroll down to the very bottom, copy and paste these lines...

@reference=128
@tmaterial=interface
b_ctonga_standard			gbtonga_standard		0	0	128	128
b_ctonga_weapon			gbtonga_weapon		0	0	128	128
b_ctonga_sensor			gbtonga_sensor		0	0	128	128
b_ctonga_assault			gbtonga_assault		0	0	128	128
b_ctonga_total			gbtonga_total		0	0	128	128
@reference=512
ctonga_totalw1			tongawireframe		0	0	128	128
ctonga_sensorw1			tongawireframe		128	0	128	128
ctonga_assaultw1			tongawireframe		256	0	128	128
ctonga_weaponw1			tongawireframe		384	0	128	128
ctonga_standardw1			tongawireframe		0	128	128	128

save the file...

next open up the tech1.tt located in the techtree folder, now copy and paste these lines in. They can go 
anywhere but most people prefer to place them amongst the other cardassian entries...

ctonga_standard 2 cyard2.odf cresear.odf
ctonga_total 2 cyard2.odf cresear.odf
ctonga_sensor 2 cyard2.odf cresear.odf
ctonga_weapon 2 cyard2.odf cresear.odf
ctonga_assault 2 cyard2.odf cresear.odf

save the file...

finally open up your cyard2.odf located in the odf/stations folder, go down to the build list and you
will see a list of the ships buildable there (check for cbattle if you can find it). Add these lines under
the cfrigate entry

buildItem1 = "ctonga_standard"
buildItem2 = "ctonga_sensor"
buildItem3 = "ctonga_assault"
buildItem4 = "ctonga_weapon"
buildItem5 = "ctonga_total"

you should now notice the numbers after the word "item" are no longer in sequence, fix this so the run from zero onwards.

save the file...

(this one is entirely optional and wont affect the ship ingame)If you like you can add these ships to your 
buildmenu for map editing if you like, just open ec_comba.odf located in the odf/other folder and add which 
ships you like, here are the lines...

item1 = "ctonga_standard"
item2 = "ctonga_sensor"
item3 = "ctonga_assault"
item4 = "ctonga_weapon"
item5 = "ctonga_total"

save the file...

Done, should be ingame and working fine.


Additional Information**

It's a very low poly model, the standard version is 650 polies and the total is 1050 polies, it uses
3 high res textures with lightmaps and comes with Borgified equivilents.

The sod and textures will work not in armada 1.

Feel free to use this in any mod so long as credit is given to me for the model
and textures. 

Feel free to edit the textures/model/odfs in any way so long as credit is given.

In the extra folder you will find a 3ds of the total variant as well as an ms3d complete with node structure, 
please feel free to play with it and release what you like.



Legal Stuff**

The material submitted with this readme is in no way connected to, or affiliated 
with Activision, its employees, representatives, consortiums, or other bodies 
directly or indirectly associated with the afore mentioned company. Therefore 
if the files contained in this mod cause damage to your system in any way then 
Activision cannot be held responsible or liable.

USE AT YOUR OWN RISK.



Credits**

Me....

Oh and Activision for a great design and awesome game.

Filefront in it&apos;s new incarnation, welcome back!

Dan1025 for the great screenshots



Contact**

Thanks, achilles

wrathofachilles@hotmail.com 