This is a new Cardassian figher design, made by kitbashing Zorgs Hideki Class. The model has 3 textures and a poly count of 421.

Included in this mod are:

SOD file
Ship textures
Borg textures
Buildbutton
Ship ODF
Weapon ODF's
Wireframe
AdmiralsLog picture

****************************************************************************************************************************************************************************************************************

Installation Instructions:

1. Place "cfighter.sod" into the Activision/Star Trek Armada II/SOD folder.
2. Place all files found in the RGB folder into the Activision/Star Trek Armada II/Textures/RGB folder.
3. Place "cfighter.odf" into the Activision/Star Trek Armada II/odf/ships folder.
4. Place the ODF files found in the pulse folder into the Activision/Star Trek Armada II/odf/weapons/pulse folder.
5. Place the "cfighter.bmp" file found in the ShipImages folder into the Activision/Star Trek Armada II/bitmaps/AdmiralsLog/ShipImages folder.
6. Find the file named "gui_global.spr" found in the Activision/Star Trek Armada II/Sprites folder and open it (use notepad).

Search for where it says:

"Cardassian build buttons"

and underneath where it says:

"@reference=64"

add:

b_cfighter	GBcfighter	0	0	64	64

Now search for where it says:

"Cardassian Wireframes"

and underneath where it says:

"@reference=64"

add:

cfighterw1			WFcfighter	0	0	64	64
cfighterw2			WFcfighter	0	0	64	64
cfighterw3			WFcfighter	0	0	64	64
cfighterw4			WFcfighter	0	0	64	64
cfighterw5			WFcfighter	0	0	64	64

Save and close the file.

7. Find the file named "tech1.tt" in the Activision/Star Trek Armada II/techtree folder and open it (use notepad).

Underneath where it says:

"Cardassian Ships"

add:

cfighter.odf 0

Save and close the file.

8. Find the file named "fulltech.tt" in the Activision/Star Trek Armada II/techtree folder and open it (use notepad).

At the top of the file add:

cfighter.odf 0

Save and close the file.

9. Open the name of whatever station you want to add the ship to as a buildable item (if any).

Add at the bottom of the list of buildable items:

buildItemXX = "cfighter" (where XX is the number after the last one on the list).

Save and close the file.

****************************************************************************************************************************************************************************************************************

Credits & Thanks:

Credit for the original model used (Hideki Class) goes to Zorg
Credit for the orginal borg texture I used goes to "Scorpians" altered SFC stock sphere mod

Thanks to Rich (thunderfoot006) for coming up with the class name and writing the tooltip.

A big thanks to Activision for releasing this game and giving us all something fun to mod and improve upon :)

If you want to use this mod for something you plan to release, you can always e-mail me at: 

dan_ocean@hotmail.co.uk

Hope you enjoy the mod! :)