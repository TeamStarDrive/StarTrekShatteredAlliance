ECHOES OUT OF TIME  -  a Federation / Babylon 5 crossover story chain
===================================================================

HOW TO INSTALL
  1. Close the game and the editor.
  2. Double-click Install_Echoes_Chain.bat.  It expects the mod at
         C:\Games\StarDrivePlus64\Mods\Star Trek
     (if yours is elsewhere, drag the mod folder onto the .bat file).
  3. Start the game fresh (new game - the story sites are placed during play, but the new
     tech and buildings only load at start-up).
  Every file it changes is backed up first to  "Test Reports and Backups\echoes_chain_<time>".
  Undo_Echoes_Chain.bat removes it again.

THE STORY (every step is something the player does)
  1. RESEARCH   Chroniton Detection  (Physics, after Tachyon Scanning, 3200 RP)
                unlocks the Chroniton Observatory.
  2. BUILD      Chroniton Observatory (600 PP, 3 upkeep, one per empire).
                Building it fires "The Chroniton Observatory Is Online": a time vortex has
                opened and the Temporal Debris Field appears on a random unowned habitable
                planet, guarded by 2 defence drones.  (The planet is named in the popup.)
  3. EXPLORE    Temporal Debris Field (land troops):
                  55%  Wreckage From Another Time  - Starfury data, 150 credits
                  30%  The Wreckage Fights Back    - Starfury data, 3 more drones
                  15%  A Fading Echo               - nothing yet, the site comes back (retry)
                Either of the first two unlocks the hidden "legendery tech" (Earthforce
                Fighter Salvage: Starfury hull, shield bonus) and places the Chronal Rift Scar.
  4. EXPLORE    Chronal Rift Scar:
                  70%  The Rift Gives Up Its Secrets - Omega-class Destroyer Schematics
                       (hidden tech mk2), an artifact, +2% research
                  30%  Echoes Ambush the Team        - the same schematics, but 4 troops
                       (2 drones, 2 walkers) and Remnant-style heavy ships in orbit
                Places the Vortex Core.
  5. FINALE     Vortex Core: "The Omega Arrives".  You receive a free Omega-class destroyer
                (the design "omega 1"), Shadow and Excalibur Programme Data (hidden tech mk3),
                500 credits, +5% research and an artifact.  The chain ends.

THE LEGENDARY TREE  (already in the mod, now named properly)
  legendery tech      Earthforce Fighter Salvage           Starfury hull
  legendery tech mk2  Omega-class Destroyer Schematics     Omega Destroyer, Shadow Fighter
  legendery tech mk3  Shadow and Excalibur Programme Data  Shadow Scout, Excalibur
  The discovered techs still have to be researched, one after the other (3000 / 5000 RP...);
  the Omega at the end of the chain is a free ship, so the player gets it regardless.

THINGS TO CHECK IN YOUR FIRST TEST (I could not run the game)
  - the tech appears under Tachyon Scanning and unlocks the building;
  - the popup after building names a planet, and the Debris Field is there;
  - the free ship "omega 1" appears at the end (if not, look in blackbox.log for "omega 1");
  - sites are only placed on unowned habitable planets; chances apply per explore.
  Tell me what the log says and I will adjust it.

FILES
  Technology\Physics\Chroniton Detection.xml      new tech
  Technology\Physics\Tachyon Scanning.xml         edited: links the new tech (installer does it)
  Buildings\Events\*.xml                          Observatory + 3 sites
  Exploration Events\*.xml                         the 4 events
  GameText.yaml                                    new text 40000-40021, plus the 6 legendary tech names
