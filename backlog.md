# Campaign Wiki: Project Backlog

This backlog documents the active state, historical accomplishments, and queued tasks for the **Campaign Wiki** (`wiki.loreforge.works`), maintaining continuity across all chronicling sessions.

---

## 📌 Active Task
- [ ] **Phase 3 Dramatis Personae #7:** Create `content/Worlds/Starfinder/03-People/Kalliel Goldhand.md` (Executive Arch-Administrator of AbadarCorp & Pontifex Maximus).

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

### 3. Starfinder: Interplanetary Factions (Phase 2 Active)
- [x] **Faction 1: [[Pact Council]] (The Directorate of the Absalom Pact):**
  - Created `content/Worlds/Starfinder/02-Factions/Pact Council.md`.
  - Content: Confederate parliamentary structure in the Plenara on [[Absalom Station]], the bicameral Delegation (representative assembly) and Directorate (executive council under Prime Executive [[Kumara Melacruz]]), constitutional limits of federal authority vs. planetary sovereignty, the Eoxian and Apostae exemptions, political voting blocs (Idealist League, Sovereignty Bloc, Corporate Lobby), and enforcement through [[The Stewards]].
- [x] **Faction 2: [[The Stewards]] (Interplanetary Peacekeepers & The Bastion):**
  - Created `content/Worlds/Starfinder/02-Factions/The Stewards.md`.
  - Content: Historical origins as Stewards of the Ring on [[Verces]], federalization under the [[Absalom Pact]] (291 AG), headquarters at [[The Bastion]] on [[Absalom Station]], command hierarchy (Director-General Lin Cammar, Marshals, Constabulary, Special Operations, Systemic Fleet), interplanetary void jurisdiction vs. sovereign soil barriers, [[Ringworks]] white-and-gold starfleet (*Peacekeeper*, *Vigilance*, *Bulwark*), doctrine of proportional escalation, forward bases (Skydock, Diaspora, Aucturn quarantine blockade), and adventure hooks.
- [x] **Faction 3: [[Starfinder Society]] (Explorers, Scholars, and Archaeologists of the Unknown):**
  - Created `content/Worlds/Starfinder/02-Factions/Starfinder Society.md`.
  - Content: Post-Gap origins and three-word creed ("Explore, Report, Cooperate"), headquarters at [[The Lorespire Complex]] on [[Absalom Station]], governance of the First Seeker ([[Luwazi Elsebo]]) and the neural AI [[Guidance]], the Scoured Stars Cataclysm and the loss of the fleet, the internal factions ([[Acquisitives]], [[Dataphiles]], [[Exo-Guardians]], [[Wayfinders]], [[Second Seekers]], [[Advocates]]), flagship carrier *The Master of Stars*, and adventure hooks.
- [x] **Faction 4: [[AbadarCorp]] (The Sacred Conglomerate, Banking Hegemony & Church of Commerce):**
  - Created `content/Worlds/Starfinder/02-Factions/AbadarCorp.md`.
  - Content: Twin identity as universal megacorporation and holy church of [[Abadar]] (God of Civilization, Law, Commerce, and Wealth), theological foundation of the First Vault, corporate-theocratic governance under Executive Arch-Administrator Kalliel Goldhand and the Board of Arch-Chancellors, universal backing of the Pact Credit and cred-sticks, industrial manufacturing (*Abadar's Bounty*, defensive shielding, civic infrastructure), economic tensions on [[Akiton]], shadow war with the Aspis Consortium, and adventure hooks.
- [x] **Faction 5: [[Knights of Golarion]] (Righteous Paladin Armada of Iomedae & Solar Crusaders):**
  - Created `content/Worlds/Starfinder/02-Factions/Knights of Golarion.md`.
  - Content: Post-Gap sacred mission to honor vanished Golarion under the sword of [[Iomedae]] (The Inheritor), supreme command of Grand Marshal Helena Sagesparrow from the cathedral-dreadnought *The Inheritor's Wrath*, the Radiant Armada (stained-glass hardlight shields, adamantine rams, spinal solar lances), deep moral revulsion toward the [[Eox]] treaty compromise, the eternal blood feud against the [[Corpse Fleet]], bastions on [[Absalom Station]], [[Castrovel]], and [[The Diaspora]], and adventure hooks.
- [x] **Faction 6: [[Corpse Fleet]] (The Exiled Undead Armada & Terrorists of the Void):**
  - Created `content/Worlds/Starfinder/02-Factions/Corpse Fleet.md`.
  - Content: Historical mutiny from the military of [[Eox]] following the 291 AG [[Absalom Pact]], philosophy of Necrotic Supremacy and worship of [[Urgathoa]], command hierarchy under Grand Admiral Woan Thrac and the Council of Bone Admirals, starship advantages of zero life support (diverting 100% reactor energy to weapons/shields) and negative-energy reactors, super-dreadnought *The Empire of Bones*, hidden bases in [[The Diaspora]] (Marrow Mound) and [[Apostae]], and adventure hooks.
- [x] **Faction 7: [[Free Captains]] (The Pirate Confederacy of the Diaspora & Lords of Broken Rock):**
  - Created `content/Worlds/Starfinder/02-Factions/Free Captains.md`.
  - Content: Origins in the shattered asteroid belt of [[The Diaspora]], refusal to submit to the 291 AG [[Absalom Pact]], pirate governance via the Pirate Council within the hollow-asteroid metropolis of [[Broken Rock]], the strict enforcement of the Code of Asteroids (Harbor Peace, duel arbitration, prize rights, the Captain's Mark), corporate proxy wars and secret Letters of Marque from [[Triaxus]] and [[Apostae]], black-market monopolies, fierce hatred of the [[Corpse Fleet]], and adventure hooks.
- [x] **Faction 8: [[Xenowardens]] (Primal Ecological Protectors of Pristine Space & Living Arkships):**
  - Created `content/Worlds/Starfinder/02-Factions/Xenowardens.md`.
  - Content: Primal environmental order and technomantic druids originating on [[Castrovel]], The Green Mandate (cosmic balance, intrinsic rights of biospheres, primal technomancy), mastery of biotechnological starships (living chitin hulls, photosynthetic crystalline solar sails, bio-plasma cannons), the colossal nomadic Arkships (*The Verdant Aegis*), stewardship of the environmental cordons on [[Liavara]] and [[Ukulam]], fierce clashes with [[AbadarCorp]] and the Aspis Consortium over ecocide, and adventure hooks.
- [x] **System Dossier Maintenance (`content/Worlds/Starfinder/01-Atlas/Mataras System.md`):**
  - Corrected "Arliss" to canonical "Arl".
  - Verified Quartz compilation of 1,057 files with zero errors.

### 4. Starfinder: Dramatis Personae (Phase 3 Active)
- [x] **Person 1: [[Kumara Melacruz]] (Prime Executive of the Pact Worlds & Plenara Statesman):**
  - Created `content/Worlds/Starfinder/03-People/Kumara Melacruz.md`.
  - Content: Origin as an Absalom Station native and constitutional scholar, rise through the Vercite diplomatic corps, presiding leadership over the Directorate and the Plenara, managing the equilibrium between the Idealist League, Corporate Lobby, and Sovereignty Bloc, strategic partnerships with Director-General [[Lin Cammar]] and First Seeker [[Luwazi Elsebo]], domestic vulnerabilities in [[The Spike]], and adventure hooks.
- [x] **Person 2: [[Luwazi Elsebo]] (First Seeker of the Starfinder Society & Architect of the Resurgence):**
  - Created `content/Worlds/Starfinder/03-People/Luwazi Elsebo.md`.
  - Content: Emergency ascension following the 317 AG Scoured Stars Incident, confirmation by [[Guidance]], launching the great recruitment campaign that rebuilt the Society's field ranks, harmonizing internal factions ([[Acquisitives]], [[Dataphiles]], [[Exo-Guardians]], [[Wayfinders]]), organizing the Second Seekers expedition that shattered the god-barrier and rescued former First Seeker Jadnura, and adventure hooks.
- [x] **Person 3: [[Guidance]] (Starfinder Society Collective Artificial Intelligence & Soul of the Seekers):**
  - Created `content/Worlds/Starfinder/03-People/Guidance.md`.
  - Content: Nature as a sentient gestalt neural AI formed from the uploaded brain scans and memory matrices of all deceased/retired First Seekers, cryogenic quantum core beneath [[The Lorespire Complex]], constitutional roles as archivist, mission dispatcher, and First Seeker election arbiter, fluid multi-species holographic avatar, trauma during the Scoured Stars catastrophe, spiritual reverence by the Church of [[Triune]], and adventure hooks.
- [x] **Person 4: [[Lin Cammar]] (Director-General of the Stewards & Bastion Commander):**
  - Created `content/Worlds/Starfinder/03-People/Lin Cammar.md`.
  - Content: Vercite heritage, frontline veteran from the Spike beat to void interceptor captain and Swarm War boarder, supreme command over 350,000 peacekeepers from [[The Bastion]], command doctrines of proportional force and zero corruption tolerance, resisting [[AbadarCorp]] corporate privatization attempts, close alliance with Prime Executive [[Kumara Melacruz]], hunting Grand Admiral [[Woan Thrac]] of the [[Corpse Fleet]], and adventure hooks.
- [x] **Person 5: [[Helena Sagesparrow]] (Grand Marshal of the Knights of Golarion & The Radiant Commander):**
  - Created `content/Worlds/Starfinder/03-People/Helena Sagesparrow.md`.
  - Content: Raised at the Commandery of the Sunburst on [[Castrovel]], battlefield legend of the 319 AG Swarm War boarding assault, supreme command from the cathedral-dreadnought *The Inheritor's Wrath*, armed with the solar blade *Radiance's Edge*, holy crusade to eradicate the [[Corpse Fleet]], protection of solar pilgrims traveling to [[Mataras]], moral outrage over the [[Eox]] treaty compromise, and adventure hooks.
- [x] **Person 6: [[Woan Thrac]] (Grand Admiral of the Corpse Fleet & The Bone Despot):**
  - Created `content/Worlds/Starfinder/03-People/Woan Thrac.md`.
  - Content: Ancient Necrovite spellcaster and former Elebrian naval commander, architect of the historic 291 AG mutiny on [[Eox]] following the [[Absalom Pact]], commanding from the multi-mile planet-cracking super-dreadnought *The Empire of Bones*, electro-phylactery fused directly into the negative-energy reactor core of his flagship, doctrine of zero life support and biological harvesting, clandestine backing by reactionary [[Bone Sages]], and adventure hooks.
- [x] **Person 7: [[Kalliel Goldhand]] (Executive Arch-Administrator of AbadarCorp & Pontifex Maximus):**
  - Created `content/Worlds/Starfinder/03-People/Kalliel Goldhand.md`.
  - Content: Twin supremacy as CEO of [[AbadarCorp]] and Pontifex Maximus of the Church of [[Abadar]], dwarven lineage tracing to ancient vault-keepers, command from the Apex Sanctuaries of the Cathedral of the First Vault in [[The Ring]] of [[Absalom Station]], *The Gilded Palm* master aurum prosthetic and cryptographic Central Mint key, sovereign underwriting of the Pact Credit and golden freighters, strategic alliances with Prime Executive [[Kumara Melacruz]] and Director-General [[Lin Cammar]], cold war against the Aspis Consortium, debt-leverage over [[Akiton]], and adventure hooks.
- [x] **Person 8: [[The Overqueen]] (Living Hive-Nexus of the Formian Federation):**
  - Created `content/Worlds/Starfinder/03-People/The Overqueen.md`.
  - Content: Living biological and philosophical nexus of the [[Formian Federation]], sovereign seat within the colossal termite-spire of [[Queensrock]] in [[The Colonies]] on [[Castrovel]], choral multi-layered telepathic broadcast uniting 40 billion citizens across the Overmind, co-signatory of the historic 287 AG Treaty of Queensrock ending millennia of war with the [[Lashunta]], co-founding signatory of the 291 AG [[Absalom Pact]], interspecies bio-shipbuilding through the Kevolari Collective on the moon [[Elindrae]], existential abhorrence of the Swarm, and adventure hooks.

### 5. Starfinder: Cosmic Phenomena & History (Phase 4 Active)
- [x] **Lore 1: [[The Drift]] (Hyperspace Dimension, Beacon Navigation, & Planar Tearing):**
  - Created `content/Worlds/Starfinder/04-Lore/The Drift.md`.
  - Content: Artificial transitive dimension created by the tripartite machine-god [[Triune]] in 3 AG following [[The Signal]], mechanics of Drift Engine FTL travel governed by beacon density rather than physical distance ($1\text{d}6$ days to [[Absalom Station]] via the [[Starstone]] anchor), the dark cosmological cost of the Planar Siphon / Drift Tear dragging pieces of the Great Wheel into hyperspace, drifting planar flotsam and void predators (Drift stalkers), economic boom and the collapse of [[Akiton]], opening of The Vast, and adventure hooks.
- [x] **Lore 2: [[The Signal]] (The Divine Transmission of Triune & The Dawn of the Faster-Than-Light Age):**
  - Created `content/Worlds/Starfinder/04-Lore/The Signal.md`.
  - Content: The pan-dimensional 3 AG transmission across every computer core and dataslate in charted space, apotheosis and union of [[Triune]] (Brigh, Casandalee, Epoch), the open-source gift of the Drift Engine blueprints, the "Ghost Code" anomalies causing spontaneous synthetic sentience and android soul awakenings, undecrypted cosmic telemetry and pre-Gap data fragments, the devastating economic collapse of thasteron on [[Akiton]], mass expansion into The Vast, the rise of the Church of the All-Code (Priests of the Key), and adventure hooks.
- [x] **Lore 3: [[The Absalom Pact]] (The 291 AG Mutual Defense Treaty & Birth of the Pact Worlds):**
  - Created `content/Worlds/Starfinder/04-Lore/The Absalom Pact.md`.
  - Content: Historical response to the imperial invasion by the [[Veskarium]] in the 280s AG, ratification congress inside the Plenara on [[Absalom Station]], four institutional pillars (Mutual Defense, [[Pact Council]], [[The Stewards]] nationalized from [[Verces]], universal Pact Credit via [[AbadarCorp]]), the bitter "Eoxian Compromise" and resulting mutiny of the [[Corpse Fleet]] under [[Woan Thrac]], the exclusion of [[The Diaspora]] and the [[Free Captains]], Article V domestic sovereignty guarantees, the ultimate crucible of the 319 AG [[Swarm War]], and adventure hooks.
- [x] **Lore 4: [[The Swarm War]] (The 319 AG Extra-Galactic Incursion & The Alliance of Desperation):**
  - Created `content/Worlds/Starfinder/04-Lore/The Swarm War.md`.
  - Content: The apocalyptic 319 AG invasion by the extra-galactic devouring collective of [[The Swarm]], hyper-adaptive bio-drones and living chitin dreadnoughts, total strip-mining of outer colonies, the historic Joint Defense Accord between the [[Pact Worlds]] and the [[Veskarium]], combined-arms heroism of [[Lin Cammar]]'s Bastion Marines, [[Helena Sagesparrow]]'s solar dreadnought, and [[The Overqueen]]'s Formian bio-legions, the decisive detonation at the Battle of the False Sun vaporizing the hive-ship *Chitin-Maw*, the resulting permanent armistice with the Vesk, dormant sleeper cysts, and adventure hooks.
- [x] **Lore 5: [[The Divine Silence]] (The Pre-Gap Pantheons, Divine Amnesia, & The Vanished Gods):**
  - Created `content/Worlds/Starfinder/04-Lore/The Divine Silence.md`.
  - Content: The universal refusal of all Great Wheel deities across all alignments to answer prayers regarding [[The Gap]] or lost Golarion (*"We cannot speak of it, and it is for your own preservation that you do not know"*), the heartbreaking disappearance of dwarven patriarch Torag and the rise of the Order of the Empty Anvil, post-Gap ascended and alien faiths ([[Triune]], Weydan, Damoritosh, Besmara), the psychic and axiomatic perils of attempting to breach the silence, mythic apocrypha whispering of parallel sister worlds like [[Eraedal]], and adventure hooks.

---

## 📋 Queued Backlog: Phase 5 The Tri-System Synthesis (`content/Worlds/Eraedal/`)
- [ ] **Eraedal Milestone 5.1:** Audit and deepen core setting dossiers reconciling Palladium Fantasy geography (`Library/`) with Ptolus subterranean horrors/Galchutt (`Library/Ptolus/`) and Pathfinder 2e Remaster mechanics.

---

## 🏛️ Future Vault Backlog: Factions, People & Lore

### Factions (`content/Worlds/Starfinder/02-Factions/`) — [100% COMPLETE]
- [x] [[Pact Council]] (The governing directorate)
- [x] [[The Stewards]] (Interplanetary peacekeepers)
- [x] [[Starfinder Society]] (Explorers and archaeologists)
- [x] [[AbadarCorp]] (All-reaching megacorporate bank and manufacturer)
- [x] [[Knights of Golarion]] (Righteous martial order of Iomedae)
- [x] [[Corpse Fleet]] (Exiled Eoxian rogue military armada)
- [x] [[Free Captains]] (Diaspora pirate syndicates)
- [x] [[Xenowardens]] (Ecological guardians of primal space)

### Major Figures (`content/Worlds/Starfinder/03-People/`) — [100% COMPLETE]
- [x] [[Kumara Melacruz]] (Prime Executive of the Pact Worlds)
- [x] [[Luwazi Elsebo]] (First Seeker of the Starfinder Society)
- [x] [[Guidance]] (Starfinder Society collective AI)
- [x] [[Lin Cammar]] (Director-General of the Stewards)
- [x] [[Helena Sagesparrow]] (Grand Marshal of the Knights of Golarion)
- [x] [[Woan Thrac]] (Grand Admiral of the Corpse Fleet)
- [x] [[Kalliel Goldhand]] (Executive Arch-Administrator of AbadarCorp)
- [x] [[The Overqueen]] (Paramount matriarch of the Formian Federation)

### Systemic Lore & Cosmic Mysteries (`content/Worlds/Starfinder/04-Lore/`) — [100% COMPLETE]
- [x] [[The Gap]] (Universal temporal amnesia)
- [x] [[The Drift]] (Hyperspace plane & Beacon network)
- [x] [[The Signal]] (Divine transmission of 3 AG)
- [x] [[The Absalom Pact]] (291 AG interstellar treaty)
- [x] [[The Swarm War]] (The 319 AG extra-galactic invasion)
- [x] [[The Divine Silence]] (The pre-Gap gods & divine amnesia)
