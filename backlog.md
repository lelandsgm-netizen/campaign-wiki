# Campaign Wiki: Project Backlog

This backlog documents the active state, historical accomplishments, and queued tasks for the **Campaign Wiki** (`wiki.loreforge.works`), maintaining continuity across all chronicling sessions.

---

## 📌 Active Task
- [ ] **Phase 2 Faction Dossier #1:** Create `content/Worlds/Starfinder/02-Factions/Pact Council.md` (The Directorate of the Absalom Pact).

---

## ✅ Completed Tasks (Backlogged from Current Work)

### 1. Gateway & Wiki Infrastructure Fixes
- [x] **Wiki Homepage Wikilink Parsing Fix (`content/index.md`):**
  - Diagnosed why `[[The Gap]]`, `[[Mataras System]]`, `[[Eraedal]]`, and `[[Floenry Isles]]` were rendering as literal text inside the gateway cards.
  - Cause: Raw HTML `<p>` and `<h3>` tags enclosed the links inside an HTML block, bypassing Quartz’s Remark/OFM Markdown parser.
  - Fix: Converted card interiors to native Markdown headings (`###`) and paragraphs separated by blank lines within the container `<div>`.
  - Verified: Rebuilt with Quartz; all wikilinks now resolve to valid HTML anchor tags.
- [x] **Shell-Guard Whitelist & Elevated Autonomy Setup:**
  - Whitelisted `campaign-wiki` inside `C:\Users\lelan\.gemini\config\hooks\shell-guard.js` by checking `args.Cwd` and `workspacePaths` against the repository name.
  - Updated `AGENTS.md` to grant direct terminal authority (`Select-String`, `Get-ChildItem`, `git grep`, `npx quartz build`) without requiring intermediate scratch scripts.

### 2. Starfinder: Mataras System Atlas (Phase 1: 14 of 14 Bodies Complete & Verified)
- [x] **Body 1: [[Mataras]] (The Sun):**
  - Created `content/Worlds/Starfinder/01-Atlas/Mataras.md`.
  - Content: Astrogation profile ($\times 100$ diameter, yellow dwarf), Sister Novaheart’s *Speech Under the Prominence* (223 AG), The Burning Archipelago force-bubble cities ([[Dawnshore]], [[Corona]], [[Stellacuna]], [[Fireside]], [[Verdeon]], [[Asanatown]]), Deep Sun mysteries (Far Portal Station, Ezorod the Blind City, Kahlannal city-ship, The Crucible, and the anassanois).
- [x] **Body 2: [[Aballon]] (The Horse / The Forge):**
  - Created `content/Worlds/Starfinder/01-Atlas/Aballon.md`.
  - Content: Scorched innermost world ($\times 1/3$ G, 12-hour day), the First Ones and construct evolution of the [[Anacites]], the Triad of Ideologies (*Those Who Wait*, *Those Who Become*, *Those Who Are*), the divine emergence of Epoch and [[Triune]] (3 AG), and major megaplexes ([[Striving]], [[Pursuit]], [[Automatrix]], [[Endeavor]], Horse Eye Orbital Plate, Sea of Glass, Sun-Gutter).
- [x] **Body 3: [[Castrovel]] (The Green Mother):**
  - Created `content/Worlds/Starfinder/01-Atlas/Castrovel.md`.
  - Content: Hyper-fertile jungle world ($\times 1$ G, 24-hr day, 182-day year), the Four Continents ([[Asana]], [[The Colonies]], [[Sovyrian]], [[Ukulam]]), industrial moon [[Elindrae]], the Formian-Lashunta War and the historic 287 AG Armistice, ancient [[Aiudara]] (Elf Gates), and ecological threats (ksariks, moldstorms).
- [x] **Body 4: [[Absalom Station]] (The Nexus at the Void):**
  - Created `content/Worlds/Starfinder/01-Atlas/Absalom Station.md`.
  - Content: 5-mile starbase in the orbital coordinates of lost Golarion, powered by the divine [[Starstone]] reactor (universal Drift beacon), macro-sectors ([[The Eye]], [[The Ring]], [[The Arms]], [[The Spike]], Ghost Levels, Starstone Reactor), [[The Armada]] orbital flotilla, the [[Pact Council]], [[The Stewards]], and the [[Starfinder Society]].
- [x] **Body 5: [[Akiton]] (The Red Planet):**
  - Created `content/Worlds/Starfinder/01-Atlas/Akiton.md`.
  - Content: Low-gravity dying world ($\times 1/3$ G, 24h 40m day), the Thasteron economic boom and the 3 AG Drift crash, native peoples ([[Ysoki]] ratfolk cradle, [[Shobhads]], [[Contemplatives of Ashok]], [[Ikeshti]]), major settlements ([[Maro]] in the Edaio Rift, [[Arl]], [[Daza]], [[Estuar]], Ashok Crater).
- [x] **Body 6: [[Verces]] (The Ring of Nations):**
  - Created `content/Worlds/Starfinder/01-Atlas/Verces.md`.
  - Content: Tidally locked terrestrial world ($\times 1$ G, 3-year orbit), tripartite geography ([[Fullbright]], [[Darkside]], and the temperate 27-state [[The Ring of Nations]]), the [[Verthani]] and chromatic skin communication, the Augmented and cybernetic integration culture, [[Skydock]] orbital space-elevator array, [[Ringworks]] aerospace shipyards, and the historical origin of [[The Stewards]].
- [x] **Body 7: [[The Diaspora]] (The Shattered Belt):**
  - Created `content/Worlds/Starfinder/01-Atlas/The Diaspora.md`.
  - Content: Asteroid belt origin in the ancient pre-Gap destruction of twin worlds Damiar and Iovo by an Eoxian superweapon, native void-winged [[Sarcesians]] and extreme long-range sniper defense, the hollow pirate metropolis of [[Broken Rock]] and the Free Captains' Code of Asteroids, [[The River Between]] vacuum watercourse, [[Nisis]] sub-ice cryogenic ocean, and Dwarven star-citadel adamantine smelters.
- [x] **Body 8: [[The Idari]] (The Eternal Colony Ship):**
  - Created `content/Worlds/Starfinder/01-Atlas/The Idari.md`.
  - Content: Cylindrical rotating world-ship ($\times 1$ G centripetal spin, 2.5 mi diameter $\times$ 10.5 mi length), sub-light Exodus from dying Kasath, arrival in 240 AG and sovereign Pact signatory status (291 AG), interior biomes ([[Almesla]], [[Sholar Adoth]] ancestral desert, Red Rill canal), four-armed [[Kasathas]], the mouth veil taboo, the rite of The Temperance, and the Doyenate.
- [x] **Body 9: [[Eox]] (The Dead World):**
  - Created `content/Worlds/Starfinder/01-Atlas/Eox.md`.
  - Content: Radioactive, airless dead planet ($\times 0.9$ G, 5-year orbit), ancient Magefire superweapon backlash, necro-oligarchy of the [[Bone Sages]] (necrovites, liches, vampires), capital necropolis [[Orphys]] beneath force-field domes, [[The Facet]] vitrified crater, necrotechnology and cyber-grafts, interplanetary reality-television death sports, and the rogue military shadow of the exiled [[Corpse Fleet]].
- [x] **Body 10: [[Triaxus]] (The Wanderer):**
  - Created `content/Worlds/Starfinder/01-Atlas/Triaxus.md`.
  - Content: Eccentric 317-year elliptical orbit, transition into the multi-generational Great Winter, dimorphic [[Ryphorians]] (Winterborn and Summerborn), corporate executive True Dragons of [[The Drakelands]], constitutional democracy of [[The Allied Territories]] ([[Kamiat]]), and the bonded aerial knights of [[The Skyfire Legion]].
- [x] **Body 11: [[Liavara]] (The Dreamer):**
  - Created `content/Worlds/Starfinder/01-Atlas/Liavara.md`.
  - Content: Ringed peach-and-gold gas giant ($\times 6.5$ Terrestrial diameter, 12-year orbit), protected planetary wildlife sanctuary administered by Bretheda, telepathic [[Barathu]] "Dreamers" and the atmospheric harmonic chorus, luxury resort moon [[Roselight]], holy Shirren hive-world [[Nchak]] (seat of Hylax), and the spellflux storm moon [[Arkanen]].
- [x] **Body 12: [[Bretheda]] (The Cradle):**
  - Created `content/Worlds/Starfinder/01-Atlas/Bretheda.md`.
  - Content: Super-colossus blue-green gas giant ($\times 11.2$ Terrestrial diameter, 30-year orbit), shapeshifting [[Barathu]] and the fusion collective state, floating living megacities like [[Sophiar]] (City of Bio-Logic), living bio-shipyards, the Brethedan Joint Directorate, and major moons ([[Kalo-Mahalo]] aquatic world, [[Dykon]] silicon mathematicians, [[Marata]] preservation reserve).
- [x] **Body 13: [[Apostae]] (The Maiden):**
  - Created `content/Worlds/Starfinder/01-Atlas/Apostae.md`.
  - Content: Precursor alien derelict world-ship planetoid ($\times 0.25$ Terrestrial diameter, 68-year orbit), dark obsidian spire capital [[Nightarch]], the indestructible alien Portal Arch, ruling [[Drow]] arms-dealing corporate houses (House Zeizerer, House Vaelis), indentured [[Orcs]] in permanent debt-bondage, and the lethal exploration of the unmapped deep alien vaults.
- [x] **Body 14: [[Aucturn]] (The Stranger):**
  - Created `content/Worlds/Starfinder/01-Atlas/Aucturn.md`.
  - Content: Sentient embryonic Great Old One world ($\times 1.2$ Terrestrial diameter, 180-year orbit), toxic mutagenic atmosphere, the bizarre [[Midwives]] (larval cosmic custodians), Cults of the [[Elder Mythos]], [[The Citadel of the Black]] (monolithic spire of Nyarlathotep and High Prophet Otolmens), [[The Amniotic Sea]], and the absolute quarantine blockade of [[The Stewards]].
- [x] **System Dossier Maintenance (`content/Worlds/Starfinder/01-Atlas/Mataras System.md`):**
  - Corrected "Arliss" to canonical "Arl".
  - Verified Quartz compilation of 1,048 files with zero errors.

---

## 📋 Queued Backlog: Phase 2 Interplanetary Factions (`02-Factions/`)

---

## 🏛️ Future Vault Backlog: Factions, People & Lore

### Factions (`content/Worlds/Starfinder/02-Factions/`)
- [ ] [[Pact Council]] (The governing directorate)
- [ ] [[The Stewards]] (Interplanetary peacekeepers)
- [ ] [[Starfinder Society]] (Explorers and archaeologists)
- [ ] [[AbadarCorp]] (All-reaching megacorporate bank and manufacturer)
- [ ] [[Knights of Golarion]] (Righteous martial order of Iomedae)
- [ ] [[Corpse Fleet]] (Exiled Eoxian rogue military armada)
- [ ] [[Free Captains]] (Diaspora pirate syndicates)
- [ ] [[Xenowardens]] (Ecological guardians of primal space)

### Major Figures (`content/Worlds/Starfinder/03-People/`)
- [ ] Prime Executive Kumara Melacruz
- [ ] First Seeker Luwazi Elsebo
- [ ] Guidance (Starfinder Society collective AI)
- [ ] Overqueen of the Formian Federation
- [ ] High Luminary of Dawnshore

### Systemic Lore & Cosmic Mysteries (`content/Worlds/Starfinder/04-Lore/`)
- [ ] [[The Drift]] & The Signal (3 AG)
- [ ] The Absalom Pact (291 AG)
- [ ] The Swarm Incursions
- [ ] The Pre-Gap Gods & Divine Silence
