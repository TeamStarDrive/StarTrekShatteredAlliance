~Rnara Ship Addon

~Introduction:
This ship is one of the many expected to result from the Achilles exchange. It was originally the
Rdnara class.... but somewhere along the lines the "d" disappeared XD.
The Rnara class is basically a Griffon class with pulse phasers, but it also has 
very pretty contrails with it. Included in this conversion mod are the require ship files,
a build button, admiral's log picture, and wireframe.

~Installation:
1. Copy over the files provided to thier respective locations

2. Open up tech1.tt. At the bottom, add these lines:

//Achilles Shipyard ;)
rnara.odf 0

3. Open up your favorite shipyard (preferably Romulan) and add this line:

buildItemXX = "rnara.odf"

Where XX is the number in the build list

4. Open up GUI_Global.spr and add these lines underneath the federation build buttons:

//Achilles Shipyard Stuff
@reference=64
b_rnara	rnarabuild	0	0	64	64
rnaraw1		rnarawire		0	0	64	64

5. Enjoy

~Credits:
Conversion to Armada 2 by Ultimate_Dragon
Design by Azel/Atolm
Model & Textures by WrathofAchilles/Achilles

Feel free to use the contents of this file in your own mods so long as credit is given, permission does not need to be aquired.