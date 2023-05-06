This is the 1.1 version of my Vulcan full race mod, I've fixed all of the bugs that have been reported, and even added a couple of new units. The following fixes/adjustments have been made in this version:

- Readme now includes an instruction step detailing how to avoid the race number/instantActionSlot problem.
- Freighters will now mine latinum.
- Shipyard and Advanced Shipyard now have different build costs.
- A cargo ship has been added.
- A trading station has been added.
- An upgrade research station has been added.
- A colony ship (with pod) has been added.
- Research station(s) will no longer have the spider box in is centre.
- Pulse phaser texture now included.
- Hardpoint error causing ships to be built outside of yards now fixed.
- Special weapons now assigned to ships.

Included in this mod are:

AI files
SOD files
GUI
Ship textures
Borg textures
Weapon textures
Build buttons
Special weapon buttons
Ship ODFs
Station ODFs
Weapon ODFs
Special weapon ODFs
Wireframes
Admirals Log pictures
Sounds

***************************************************************************************************************************************************************************************************************

Installation Instructions - Due to the scale of this mod these are quite extensive, however they have been tested and they work, so I urge you to please follow them VERY carefully, if you install the mod by following these instructions you will have no problems. If you encounter a problem after installation I ask that you go through the instructions again before posting on the comments section of the mod, or the forum e.t.c. If, after you are sure you've followed the instructions you still encounter problems, feel free to contact me and I will do what I can to help :)

1. Place the sod files into the Activision/Star Trek Armada II/SOD folder.

2. Place the AIP files into the Activision/Star Trek Armada II/AI/AIPs folder.

3. Place all files found in the RGB folder into the Activision/Star Trek Armada II/Textures/RGB folder.

4. Place the file in the misc folder into the Activision/Star Trek Armada II/misc folder.

5. Place the file in the sprites folder into the Activision/Star Trek Armada II/sprites folder.

6. Place the bitmap images found in the ShipImages folder into the Activision/Star Trek Armada II/bitmaps/AdmiralsLog/ShipImages folder.

7. Place the files found in the sounds/voiceover/ingame folder into the Activision/Star Trek Armada II/sounds/voiceover/ingame folder. Before you ask no there are not a load of sound files missing, there are so few in the folder because the majority of the Vulcan units use various stock sounds that work well as Vulcan voices, so they should already be in your game.

8. Place the ODF files found in the odf/ships folder into the Activision/Star Trek Armada II/odf/ships folder.

9. Place the ODF files found in the odf/stations folder into the Activision/Star Trek Armada II/odf/stations folder.

10. Place the ODF files found in the phasers folder into the Activision/Star Trek Armada II/odf/weapons/phasers folder.

11. Place the ODF files found in the photons folder into the Activision/Star Trek Armada II/odf/weapons/photons folder.

12. Place the ODF files found in the pulse folder into the Activision/Star Trek Armada II/odf/weapons/pulse folder.

13. Place the ODF files found in the special_weapons folder into the Activision/Star Trek Armada II/odf/special_weapons folder.

14. Place the ODF files found in the other folder into the Activision/Star Trek Armada II/odf/other folder. - Note that if you have already modded other races into your game you will need to open the "races.odf" file from this mod and paste the vulcan line into your own version, ensuring to adjust the race numbers accordingly.

NB - Depending on where in your "races.odf" file the vulcans are, will need to open the "vulcan.odf" file (odf/others folder) and change the "instantActionSlot" value to one less than the vulcans race number in your "races.odf" file (odf/others folder). E.g if the vulcans are race8 in your races.odf file change the "instantActionSlot" value to 7. 

Note that if you have not altered your "races.odf" file at any time (you have not added or removed any races compared to the stock version of the game) you can disregard this, as the "instantActionSlot" value is already set to the right value for your game.

15. Place the "events" file in the mods main directory into your game directory Activision/Star Trek Armada II, ensuring to click yes when the computer asks you to replace the original file - Note that this will override the events file already in your game directory, if you have made any changes to the file that you do not wish to loose you will need to open the version included in the mod (using notepad) and copy/cut and paste all of the entries containing the word "vulcan" (can be found via the "find" function in notepad) into thier corresponding locations in your "events" file.

16. Locate the file named "gui_global.spr" found in the Activision/Star Trek Armada II/Sprites folder and open it (use notepad).

Search for where it says:

"alien build buttons"

and underneath where it says:

"b_zentity			gbzships	0	0	64	64"

Leave a line and add:

# Vulcan build buttons
@reference=64
@tmaterial=default

b_vbase			GBvbase		0	0	64	64
b_vmining		GBvmining	0	0	64	64
b_vyard			GBvyard		0	0	64	64
b_vyard2			GBvyard2	0	0	64	64
b_vresear		GBvresear	0	0	64	64
b_vresear2		GBvresear2	0	0	64	64
b_vupgrade		GBvupgrade	0	0	64	64
b_vturret			GBvturret		0	0	64	64
b_vturret2		GBvturret2	0	0	64	64
b_vsensor		GBvsensor	0	0	64	64
b_vorbital			GBvorbital	0	0	64	64
b_vtrading		GBvtrading	0	0	64	64
b_vplasmk1		GBvplasmk1	0	0	64	64
b_vplasmk2		GBvplasmk2	0	0	64	64
b_vkaran			GBvkaran	0	0	64	64
b_vsonyr			GBvsonyr	0	0	64	64
b_vktra			GBvktra		0	0	64	64
b_vminta			GBvminta	0	0	64	64
b_vsotek			GBvsotek		0	0	64	64
b_vsrol			GBvsrol		0	0	64	64
b_vtmir			GBvtmir		0	0	64	64
b_vsormir		GBvsormir	0	0	64	64
b_vtran			GBvtran		0	0	64	64
b_vtran2			GBvtran2		0	0	64	64
b_vtorrol			GBvtorrol		0	0	64	64
b_vtaurik			GBvtaurik		0	0	64	64
b_vmirres		GBvmirres	0	0	64	64
b_vvreenak		GBvvreenak	0	0	64	64
b_vvultres		GBvvultres	0	0	64	64
b_vconst			GBvconst	0	0	64	64
b_vfreight			GBvfreight	0	0	64	64
b_vcargo			GBvcargo	0	0	64	64
b_vcolony		GBvcolony	0	0	64	64
b_vrepair			GBvrepair	0	0	64	64
b_vpod1			GBvpod1		0	0	64	64
b_vpod2			GBvpod2		0	0	64	64
b_vpod3			GBvpod3		0	0	64	64
b_vpod4			GBvpod4		0	0	64	64
b_vpod5			GBvpod5		0	0	64	64
b_vpod6			GBvpod6		0	0	64	64
b_vupod1			GBvupod1	0	0	64	64
b_vupod2			GBvupod2	0	0	64	64
b_vupod3			GBvupod3	0	0	64	64
b_vupod4			GBvupod4	0	0	64	64
b_vupod5			GBvupod5	0	0	64	64
b_vupod6			GBvupod6	0	0	64	64
b_vupod7			GBvupod7	0	0	64	64
b_vupod8			GBvupod8	0	0	64	64
b_vupod9			GBvupod9	0	0	64	64
b_vupod10		GBvupod10	0	0	64	64
b_gvtachyon_pod		GBvtachyon_pod	0	0	64	64
b_gvcloak_pod		GBvcloak_pod	0	0	64	64
b_gvtransmit_pod		GBvtransmit_pod	0	0	64	64
b_gvmines_pod		GBvmines_pod	0	0	64	64
b_gvhunter_pod		GBvhunter_pod	0	0	64	64
b_gvenginc_pod		GBvenginc_pod	0	0	64	64
b_gvshieldenh_pod		GBvshieldenh_pod	0	0	64	64
b_gvsendis_pod		GBvsendis_pod	0	0	64	64
b_gvpsyblst_pod		GBvpsyblst_pod	0	0	64	64
b_gvrepcrew_pod		GBvrepcrew_pod	0	0	64	64
b_gvhilaunch_pod		GBvhilaunch_pod	0	0	64	64
b_gvprecise_pod		GBvprecise_pod	0	0	64	64
b_gvplasma_pod		GBvplasma_pod	0	0	64	64

Now search for where it says:

"8472 wireframes"

and underneath the last entry:

"8472_shipupgraderesearchw5	8472wireframe04	192	192	48	48"

Leave a line and add:

#Vulcan Wireframes

@reference=64
@tmaterial=interface

vplasmk1w1	WFvplasmk1	0	0	64	64
vplasmk1	w2	WFvplasmk1	0	0	64	64
vplasmk1	w3	WFvplasmk1	0	0	64	64
vplasmk1	w5	WFvplasmk1	0	0	64	64
vplasmk1	w5	WFvplasmk1	0	0	64	64

vplasmk2w1	WFvplasmk2	0	0	64	64
vplasmk2	w2	WFvplasmk2	0	0	64	64
vplasmk2	w3	WFvplasmk2	0	0	64	64
vplasmk2	w4	WFvplasmk2	0	0	64	64
vplasmk2	w5	WFvplasmk2	0	0	64	64

vkaranw1		WFvkaran	0	0	64	64
vkaranw2		WFvkaran	0	0	64	64
vkaranw3		WFvkaran	0	0	64	64
vkaranw4		WFvkaran	0	0	64	64
vkaranw5		WFvkaran	0	0	64	64

vsonyrw1		WFvsonyr	0	0	64	64
vsonyrw2		WFvsonyr	0	0	64	64
vsonyrw3		WFvsonyr	0	0	64	64
vsonyrw4		WFvsonyr	0	0	64	64
vsonyrw5		WFvsonyr	0	0	64	64

vktraw1		WFvktra		0	0	64	64
vktraw2		WFvktra		0	0	64	64
vktraw3		WFvktra		0	0	64	64
vktraw4		WFvktra		0	0	64	64
vktraw5		WFvktra		0	0	64	64

vsotekw1		WFvsotek	0	0	64	64
vsotekw2		WFvsotek	0	0	64	64
vsotekw3		WFvsotek	0	0	64	64
vsotekw4		WFvsotek	0	0	64	64
vsotekw5		WFvsotek	0	0	64	64

vmintaw1		WFvminta	0	0	64	64
vmintaw2		WFvminta	0	0	64	64
vmintaw3		WFvminta	0	0	64	64
vmintaw4		WFvminta	0	0	64	64
vmintaw5		WFvminta	0	0	64	64

vsrolw1		WFvsrol		0	0	64	64
vsrolw2		WFvsrol		0	0	64	64
vsrolw3		WFvsrol		0	0	64	64
vsrolw4		WFvsrol		0	0	64	64
vsrolw5		WFvsrol		0	0	64	64

vtmirw1		WFvtmir		0	0	64	64
vtmirw2		WFvtmir		0	0	64	64
vtmirw3		WFvtmir		0	0	64	64
vtmirw4		WFvtmir		0	0	64	64
vtmirw5		WFvtmir		0	0	64	64

vsormirw1	WFvsormir	0	0	64	64
vsormirw2	WFvsormir	0	0	64	64
vsormirw3	WFvsormir	0	0	64	64
vsormirw4	WFvsormir	0	0	64	64
vsormirw5	WFvsormir	0	0	64	64

vtranw1		WFvtran		0	0	64	64
vtranw2		WFvtran		0	0	64	64
vtranw3		WFvtran		0	0	64	64
vtranw4		WFvtran		0	0	64	64
vtranw5		WFvtran		0	0	64	64

vtran2w1		WFvtran2	0	0	64	64
vtran2w2		WFvtran2	0	0	64	64
vtran2w3		WFvtran2	0	0	64	64
vtran2w4		WFvtran2	0	0	64	64
vtran2w5		WFvtran2	0	0	64	64

vtaurikw1		WFvtaurik	0	0	64	64
vtaurikw2		WFvtaurik	0	0	64	64
vtaurikw3		WFvtaurik	0	0	64	64
vtaurikw4		WFvtaurik	0	0	64	64
vtaurikw5		WFvtaurik	0	0	64	64

vtorrolw1		WFvtorrol	0	0	64	64
vtorrolw2		WFvtorrol	0	0	64	64
vtorrolw3		WFvtorrol	0	0	64	64
vtorrolw4		WFvtorrol	0	0	64	64
vtorrolw5		WFvtorrol	0	0	64	64

vvreenakw1	WFvvreenak	0	0	64	64
vvreenakw2	WFvvreenak	0	0	64	64
vvreenakw3	WFvvreenak	0	0	64	64
vvreenakw4	WFvvreenak	0	0	64	64
vvreenakw5	WFvvreenak	0	0	64	64

vmirresw1	WFvmirres	0	0	64	64
vmirresw2	WFvmirres	0	0	64	64
vmirresw3	WFvmirres	0	0	64	64
vmirresw4	WFvmirres	0	0	64	64
vmirresw5	WFvmirres	0	0	64	64

vvultresw1	WFvvultres	0	0	64	64
vvultresw2	WFvvultres	0	0	64	64
vvultresw3	WFvvultres	0	0	64	64
vvultresw4	WFvvultres	0	0	64	64
vvultresw5	WFvvultres	0	0	64	64
	
vfreightw1	WFvfreight	0	0	64	64
vfreightw2	WFvfreight	0	0	64	64
vfreightw3	WFvfreight	0	0	64	64
vfreightw4	WFvfreight	0	0	64	64
vfreightw5	WFvfreight	0	0	64	64

vconstw1		WFvconst	0	0	64	64
vconstw2		WFvconst	0	0	64	64
vconstw3		WFvconst	0	0	64	64
vconstw4		WFvconst	0	0	64	64
vconstw5		WFvconst	0	0	64	64

vcargow1		WFvcargo	0	0	64	64
vcargow2		WFvcargo	0	0	64	64
vcargow3		WFvcargo	0	0	64	64
vcargow4		WFvcargo	0	0	64	64
vcargow5		WFvcargo	0	0	64	64

vcolonyw1	WFvcolony	0	0	64	64
vcolonyw2	WFvcolony	0	0	64	64
vcolonyw3	WFvcolony	0	0	64	64
vcolonyw4	WFvcolony	0	0	64	64
vcolonyw5	WFvcolony	0	0	64	64

vbasew1		WFvbase		0	0	64	64
vbasew2		WFvbase		0	0	64	64	
vbasew3		WFvbase		0	0	64	64
vbasew4		WFvbase		0	0	64	64
vbasew5		WFvbase		0	0	64	64

vminingw1	WFvmining	0	0	64	64
vminingw2	WFvmining	0	0	64	64
vminingw3	WFvmining	0	0	64	64
vminingw4	WFvmining	0	0	64	64
vminingw5	WFvmining	0	0	64	64

vyardw1		WFvyard		0	0	64	64
vyardw2		WFvyard		0	0	64	64
vyardw3		WFvyard		0	0	64	64
vyardw4		WFvyard		0	0	64	64
vyardw5		WFvyard		0	0	64	64

vyard2w1		WFvyard2	0	0	64	64
vyard2w2		WFvyard2	0	0	64	64
vyard2w3		WFvyard2	0	0	64	64
vyard2w4		WFvyard2	0	0	64	64
vyard2w5		WFvyard2	0	0	64	64

vresearw1	WFvresear	0	0	64	64
vresearw2	WFvresear	0	0	64	64
vresearw3	WFvresear	0	0	64	64
vresearw4	WFvresear	0	0	64	64
vresearw5	WFvresear	0	0	64	64

vresear2w1	WFvresear2	0	0	64	64
vresear2w2	WFvresear2	0	0	64	64
vresear2w3	WFvresear2	0	0	64	64
vresear2w4	WFvresear2	0	0	64	64
vresear2w5	WFvresear2	0	0	64	64

vupgradew1	WFvupgrade	0	0	64	64
vupgradew2	WFvupgrade	0	0	64	64
vupgradew3	WFvupgrade	0	0	64	64
vupgradew4	WFvupgrade	0	0	64	64
vupgradew5	WFvupgrade	0	0	64	64

vorbitalw1	WFvorbital	0	0	64	64
vorbitalw2	WFvorbital	0	0	64	64
vorbitalw3	WFvorbital	0	0	64	64
vorbitalw4	WFvorbital	0	0	64	64
vorbitalw5	WFvorbital	0	0	64	64

vtradingw1	WFvtrading	0	0	64	64
vtradingw2	WFvtrading	0	0	64	64
vtradingw3	WFvtrading	0	0	64	64
vtradingw4	WFvtrading	0	0	64	64
vtradingw5	WFvtrading	0	0	64	64

vturretw1		WFvturret	0	0	64	64
vturretw2		WFvturret	0	0	64	64
vturretw3		WFvturret	0	0	64	64
vturretw4		WFvturret	0	0	64	64
vturretw5		WFvturret	0	0	64	64

vturret2w1	WFvturret2	0	0	64	64
vturret2w2	WFvturret2	0	0	64	64
vturret2w3	WFvturret2	0	0	64	64
vturret2w4	WFvturret2	0	0	64	64
vturret2w5	WFvturret2	0	0	64	64

vsensorw1	WFvsensor	0	0	64	64
vsensorw2	WFvsensor	0	0	64	64
vsensorw3	WFvsensor	0	0	64	64
vsensorw4	WFvsensor	0	0	64	64
vsensorw5	WFvsensor	0	0	64	64

vrepairw1		WFvrepair	0	0	64	64
vrepairw2		WFvrepair	0	0	64	64
vrepairw3		WFvrepair	0	0	64	64
vrepairw4		WFvrepair	0	0	64	64
vrepairw5		WFvrepair	0	0	64	64

Now search for where it says:

"Special weapon buttons"

and underneath where it says:

"@reference=64"

add:

b_gvtachyon		GBvtachyon_bar	0	0	64	64
b_gvcloak		GBvcloak_bar	0	0	64	64
b_gvtransmit		GBvtransmit_bar	0	0	64	64
b_gvmines		GBvmines_bar	0	0	64	64
b_gvprobe		GBvprobe_bar	0	0	64	64
b_gvhunter		GBvhunter_bar	0	0	64	64
b_gvenginc		GBvenginc_bar	0	0	64	64
b_gvshieldenh		GBvshieldenh_bar	0	0	64	64
b_gvsendis		GBvsendis_bar	0	0	64	64
b_gvpsyblst		GBvpsyblst_bar	0	0	64	64
b_gvrepcrew		GBvrepcrew_bar	0	0	64	64
b_gvecm 		GBvecm_bar	0	0	64	64
b_gvfighter		GBvfighter_bar	0	0	64	64
b_gvhilaunch		GBvhilaunch_bar	0	0	64	64
b_gvprecise		GBvprecise_bar	0	0	64	64
b_gvplasma		GBvplasma_bar	0	0	64	64
b_gvrepwav		GBvrepwav_bar	0	0	64	64

Now search for where it says:

"species8472_icon"

And underneath it add:

vulcan_icon			vguistu		0	0	64	64

Save and close the file.

17. Find the file named "tech1.tt" in the Activision/Star Trek Armada II/techtree folder and open it (use notepad).

Find where it says:

"SPECIES 8472 SPECIAL WEAPONS"

under the last entry:

"gresourceExtractionBeam.odf 0                           // species 8472 resource extraction beam"

Leave a line and add:

// ***[ VULCAN SHIPS ]**********************
//

vplasmk1.odf	1 vbase.odf
vplasmk2.odf	1 vbase.odf
vkaran.odf 	0
vsonyr.odf	1 vbase.odf
vktra.odf		4 vbase.odf vyard.odf vresear.odf vpod1.odf
vcolony.odf 	2 vyard.odf vresear.odf
vminta.odf	4 vbase.odf vyard.odf vresear.odf vpod1.odf
vsotek.odf	4 vbase.odf vyard.odf vresear.odf vpod1.odf
vsrol.odf		5 vbase.odf vyard.odf vresear.odf vpod1.odf vpod2.odf
vtmir.odf		5 vbase.odf vyard.odf vresear.odf vpod1.odf vpod2.odf
vsormir.odf	5 vbase.odf vyard.odf vresear.odf vpod1.odf vpod2.odf
vtran.odf		6 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf vpod3.odf
vtran2.odf	6 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf vpod3.odf
vtorrol.odf	7 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf vpod3.odf vpod4.odf
vtaurik.odf	7 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf vpod3.odf vpod4.odf
vmirres.odf	8 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf vpod3.odf vpod4.odf vpod5.odf
vvreenak.odf	8 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf vpod3.odf vpod4.odf vpod5.odf
vvultres.odf	9 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf vpod3.odf vpod4.odf vpod5.odf vpod6.odf
vconst.odf	1 vbase.odf
vcargo.odf	1 vtrading.odf
vfreight.odf	2 vbase.odf vmining.odf
vrepair.odf	2 vbase.odf vresear.odf

// ***[ VULCAN STATIONS ]**********************
//

vbase.odf		0
vmining.odf 	1 vbase.odf
vyard.odf 		1 vbase.odf
vyard2.odf 	3 vbase.odf vresear.odf vresear2.odf
vresear.odf 	2 vbase.odf vyard.odf
vresear2.odf 	3 vbase.odf vyard.odf vresear.odf
vupgrade.odf	4 vbase.odf vresear.odf vresear2.odf vyard2.odf
vturret.odf 	2 vbase.odf vyard.odf
vturret2.odf 	3 vbase.odf vresear.odf vresear2.odf
vsensor.odf 	2 vbase.odf vresear.odf
vorbital.odf 	2 vbase.odf vyard.odf
vtrading.odf	1 vbase.odf
vpod1.odf 	3 vbase.odf vyard.odf vresear.odf
vpod2.odf 	4 vbase.odf vyard.odf vresear.odf vpod1.odf
vpod3.odf 	5 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf
vpod4.odf 	6 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf vpod3.odf
vpod5.odf 	7 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf vpod3.odf vpod4.odf
vpod6.odf 	8 vbase.odf vyard2.odf vresear.odf vpod1.odf vpod2.odf vpod3.odf vpod4.odf vpod5.odf
vupod1.odf	1 vupgrade.odf
vupod2.odf	1 vupgrade.odf
vupod3.odf	1 vupgrade.odf
vupod4.odf	1 vupgrade.odf
vupod5.odf	1 vupgrade.odf
vupod6.odf	1 vupod1.odf
vupod7.odf	1 vupod2.odf
vupod8.odf	1 vupod3.odf
vupod9.odf	1 vupod4.odf
vupod10.odf	1 vupod5.odf
gvtachyon_pod.odf	1 vresear2.odf	// Tachyon Scanner
gvcloak_pod.odf	1 vresear2.odf	// Temporary Cloak
gvtransmit_pod.odf	1 vresear2.odf	// Covert Transmitter
gvmines_pod.odf	1 vresear2.odf	// Plasma Mines
gvprobe_pod.odf	1 vresear2.odf	// Sensor Probe
gvhunter_pod.odf	1 vresear2.odf	// Hunter Torpedo
gvenginc_pod.odf	1 vresear2.odf	// Impulse Overdrive
gvshieldenh_pod.odf 1 vresear2.odf	// Harmonic Enforcement
gvsendis_pod.odf	1 vresear2.odf	// Sensor Disruption
gvpsyblst_pod.odf	1 vresear2.odf	// Psychonic Attack
gvrepcrew_pod.odf	1 vresear2.odf	// Repair Crews
gvhilaunch_pod.odf	1 vresear2.odf	// High Yield Warheads
gvprecise_pod.odf	1 vresear2.odf	// Precision Targetting
gvplasma_pod.odf	1vresear2.odf	// Focused Plasma Beam


// ***[ VULCAN SPECIAL WEAPONS ]**************
//

gvtachyon.odf 	0 			// Tachyon Scanner
gvcloak.odf 	1 gvcloak_pod.odf		// Temporary Cloak
gvtransmit.odf 	1 gvtransmit_pod.odf	// Covert Transmitter
gvmines.odf 	1 gvmines_pod.odf		// Plasma Mines
gvprobe.odf 	0			// Sensor Probe
gvhunter.odf 	1 gvhunter_pod.odf		// Hunter Torpedo
gvenginc.odf 	1 gvenginc_pod.odf		// Impulse Overdrive
gvshieldenh.odf 	1 gvshieldenh_pod.odf	// Harmonic Enforcement
gvsendis.odf 	1 gvsendis_pod.odf		// Sensor Disruption
gvpsyblst.odf 	1 gvpsyblst_pod.odf	// Psychonic Attack
gvrepcrew.odf 	1 gvrepcrew_pod.odf	// Repair Crews
gvecm.odf 	0			// ECM
gvfighter.odf 	0			// Fighter Squadron
gvhilaunch.odf 	1 gvhilaunch_pod.odf	// High Yield Warheads
gvprecise.odf 	1 gvprecise_pod.odf	// Precision Targetting
gvplasma.odf 	1 gvplasma_pod.odf	// Focused Plasma Beam
gvrepwav.odf 	0			// Power Transfer Wave

Save and close the file.

18. Find the file named "fulltech.tt" in the Activision/Star Trek Armada II/techtree folder and open it (use notepad).

At the top of the file add:

gvtachyon_pod.odf	0
gvcloak_pod.odf	0
gvtransmit_pod.odf	0
gvmines_pod.odf	0
gvprobe_pod.odf	0
gvhunter_pod.odf	0
gvenginc_pod.odf	0
gvshieldenh_pod.odf 0
gvsendis_pod.odf	0
gvpsyblst_pod.odf	0
gvrepcrew_pod.odf	0
gvhilaunch_pod.odf	0
gvprecise_pod.odf	0
gvplasma_pod.odf	0
gvtachyon.odf 0
gvcloak.odf 0
gvtransmit.odf 0
gvmines.odf 0
gvprobe.odf 0
gvhunter.odf 0
gvenginc.odf 0
gvshieldenh.odf 0
gvsendis.odf 0
gvpsyblst.odf 0
gvrepcrew.odf 0
gvecm.odf 0
gvfighter.odf 0
gvhilaunch.odf 0
gvprecise.odf 0
gvplasma.odf 0
gvrepwav.odf 0
vvultres.odf 0
vrepair.odf 0
vcargo.odf 0
vcolony.odf 0
vpod1.odf 0
vpod2.odf 0
vpod3.odf 0
vpod4.odf 0
vpod5.odf 0
vpod6.odf 0
vupod1.odf 0
vupod2.odf 0
vupod3.odf 0
vupod4.odf 0
vupod5.odf 0
vupod6.odf 0
vupod7.odf 0
vupod8.odf 0
vupod9.odf 0
vupod10.odf 0
vbase.odf 0
vmining.odf 0
vyard.odf 0
vyard2.odf 0
vresear.odf 0
vresear2.odf 0
vupgrade.odf 0
vturret.odf 0
vturret2.odf 0
vsensor.odf 0
vorbital.odf 0
vtrading.odf 0
vplasmk1.odf 0
vplasmk2.odf 0
vkaran.odf 0
vsonyr.odf 0
vktra.odf 0
vminta.odf 0
vsotek.odf 0
vsrol.odf 0
vtmir.odf 0
vsormir.odf 0
vtran.odf 0
vtran2.odf 0
vtorrol.odf 0
vtaurik.odf 0
vmirres.odf 0
vvreenak.odf 0
vconst.odf 0
vfreight.odf 0

Save and close the file.

19. Locate the file named "weapon.spr" found in the Activision/Star Trek Armada II/Sprites folder and open it (use notepad).

Search for where it says:

"@reference=128
@tmaterial=additive"

And underneath that add:

# Vulcan Photon torpedo
wvphot 	wvphot 		0 	0 	32 	32	@anim=tex4x4

# Vulcan hunter torpedo
wvhuntorp 	wvhuntorp 	0 	0 	32 	32	 @anim=tex4x4

# Vulcan Probe
vprobe		vprobe		0	0	64	64	@anim=tex2x2

# Vulcan Phaser Flare
vflare		Xflarev		0	0	64	64	@anim=tex2x2

Now search for where it says:

"@reference= 256
@tmaterial=additive"

And underneath that add:

# Vulcan Phaser
vphaser		wvulphas		0	0	256	64	@anim=tex1x4

# Vulcan Pulse phaser
vpulse	wvpul			0	0	256	64	@anim=tex1x1

Save and close the file.

That should be all you need to get the Vulcans to work in your game :)

***************************************************************************************************************************************************************************************************************

Credits:

All combat ships - Atolm
Main texture - Atolm
MkI Plasma Drone - Achilles model (retextured)
MkII Plasma Drone - Achilles model (kibashed & retextured)
Work Bee - Achilles model (kitbashed)
Cargo Transport - Achilles model (retextured)
Repair Drone - Achilles model (kitbashed & retextured)
Starbase - Achilles model (kibashed & retextured)
Mining Station - Major A Payne model (retextured)
Colony Ship -  Original model done by Bryan, remade my Major A Payne (retextured)
Shipyards - FahreS models (retextured)
Research Stations - Achilles models (retextured & 2 kitbashed)
Turrets & Sensor Array - Achilles models (retextured)
Orbital Mining Station - Achilles model (kitbashed)
Phaser texture - Achilles
Torpedo texture - Achilles
Pulse texture - Elavatormusic
Phaser Flare texture - Elavatormusic
GUI - Elavatormusic
Special weapon buttons - MaP
Plasma Mine texture - Achilles (altered metathran texture)
Plasma Mine model - Achilles
Hunter Torpedo Texture - MaP
Repair Drone "Voice" - Ultimate Dragon

*STOCK MATERIAL USED*

Freighter model (retextured)
Construction Ship model (retextured)
Trading Station model (retextured)
Voices

Thanks:

To all those who posted advice, support and comments on the mods forum thread (http://forums.filefront.com/st-a2-modding-editing/340724-vulcan-mod.html) - I cannot thank you all enough! Without all of you the mod would never have gotten this far :)

A special thanks to ameba/DarkEnergy, for being the only person to post a detailed bug list in the error thread. Without him testing the mod and reporting bugs along the way, there would be no 1.1 version at all.

A special thanks to the members of Starbase34 that took the time to test the mod even with the various projects they're working on.

A big thanks to Activision for releasing this game and giving us all something fun to mod and improve upon.

If you'd like to use the Vulcan race or a part of it in something you'd like to release, please check the credit section above to know who you need to contact or credit for whatever you want to use. For more details you can always email me at:

dan_ocean@hotmail.co.uk

Hope you enjoy the mod! :)