# Campaign Wiki: Session Handoff Document

This document captures the current operational state, architectural conventions, and immediate next steps for the **Campaign Wiki** (`wiki.loreforge.works`), ensuring seamless continuity across developer and agent sessions.

---

## 🧭 Executive Summary & Operating Persona

- **Repository**: `campaign-wiki` (`d:\GitHub\campaign-wiki`)
- **Platform**: Personal TTRPG campaign wiki and digital garden built on **Quartz v5.0.0**.
- **Persona: Lord Coake (Coake the Mysterious)**:
  - Identity: Founder of the Cyber-Knights, veteran of the Defilers, traveler of the Megaverse.
  - Voice: Stoic, measured, sagacious, and honorable.
  - Creed: Maintain narrative depth, mechanical fidelity, rich cross-linking, and pristine formatting.
- **Operational Pacing Rule (Agreed in `/grill-me`)**:
  > [!IMPORTANT]
  > **Micro-Batches of 2 to 3 Closely Paired Files per Turn**
  > Chroniclers generate **2 to 3 related files per turn**, compile and verify immediately via `npx quartz build`, synchronize `backlog.md`, `handoff.md`, and `roadmap.md`, and present a structured summary awaiting user review before launching the next batch.

---

## 📍 Current Progress & Immediate Next Step

### Completed Pillars (100% Verified)
- **Phase 1 Atlas**: All 14 Celestial Bodies Complete & Verified.
- **Phase 1.4 Deep Dive**: All 27 Absalom Station Ecosystem Files Complete & Verified (100%).
- **Phase 2 Factions**: All 8 Major Interplanetary Factions Complete & Verified.
- **Phase 3 Dramatis Personae**: All 8 Major Figures Complete & Verified.
- **Phase 4 Cosmic Phenomena & History**: All 6 Core Lore Pillars Complete & Verified.
- **Last Verification Build**: `npx quartz build` succeeded cleanly (1,470 emitted files, 0 errors).

### 🎯 Completed Milestone: Milestone 1.4 — Absalom Station Deep Dive & Backlink Network (27/27 Files Complete — 100%)
- **Objective Achieved**: Chronicled the entire 27-file backlink ecosystem surrounding `Absalom Station.md`, resolving all missing nodes into rich, fully linked dossiers across sectors, landmarks, civic institutions, underbelly enclaves, internal Starfinder Society factions, and core immigrant ancestries.

### 🛡️ Private GM Archive: Starfinder Adventure — Guilt of the Grave World (Chapters 1–4 Complete; Chapter 5 Final)
- **Location**: `Library/Campaigns/Absalom Station/` (100% quarantined from Quartz compilation; 0 public emissions).
- **Chapter 1: Echoes from the Grave (100% Complete — 10 Files)**: Master campaign README + 10 detailed GM encounter documents.
- **Chapter 2: World of the Dead (100% Complete — 8 Files)**: Full Atraskien Shelf overland trek, Eterrina Rikutan Influence, Manor lore, and Corpse Fleet ambush.
- **Chapter 3: Halls of the Living (100% Complete — 6 Files)**: Zo! Media studios, Sabotage Soufflé, Azlanti Trenches, Telmarci rescue, and Ahmzovar's confession.
- **Chapter 4: Into the Drift (100% Complete — 5 Files)**:
  - `00 - Chapter 4 Synopsis & Prep.md` (Drift transit times, planar fragments, planar magnetite towing rigs, Amaranth chase).
  - `Encounter 4.01 - Event 1 - Malfunction (Entering the Drift).md` (Starship Cascade Faults Hazard 3, Excuba Spectra Low 4 communion/combat, Fixed Point Solarian Crystal).
  - `Encounter 4.02 - The Burning Asteroid (Plane of Fire Fragment D1-D3).md` (Burning Rockslide Hazard 2, Thermatrods Low 4, Drifting Bonfire Severe 4, Living Caldera Chase, Planar Magnetite harvest).
  - `Encounter 4.03 - Reciprocity (Amaranth Interception).md` (Cruiser Amaranth starship duel, Rigor Mortics hull breach Severe 4, Vanyra Voshin & Faceless Lieutenant Moderate 4 boss fight, Hypernerves component).
  - `Encounter 4.04 - Corsairs of the Drift (The Defiance).md` (Opa Zari parley, Cosmic Corsairs swap meet, Groggy Corsairs bar brawl Moderate 4, Afaella therapy, Cloud Nine custom paint job, Level 5).
- **Chapter 5: Robbing the Barrow (In Progress — 2 Files Complete)**:
  - `00 - Chapter 5 Synopsis & Prep.md` (Barrow rogue planet layout, Red Alert matrix, environmental parameters, reinforcement waves).
  - `Encounter 5.01 - Approaching Barrow & The Fracture (Areas E1-E3).md` (Scene 4 starship infiltration, Micrometeor Shower Hazard 3, Necroturrets Hazard 3, Loading Dock E1 Bonecrushers, Hallway E2 Mummy Wasps, Mortic Lab E3 Robots).
- **Active Task**: Next batch chronicles the deeper laboratory wings:
  - `Encounter 5.02 - Research Wings E4-E6.md` (Necrotech Lab E4 Boneflayers Moderate 5, Gef Lab E5 chemical tanks, Reanimation Lab E6).
  - `Encounter 5.03 - Facility Core E7-E10.md` (Computer Center E7 data purge, Rescuing the Living Prisoner E9, Sub-level reactor access E10).

### 🚀 Upcoming Milestone: Phase 5 — The Tri-System Synthesis (`content/Worlds/Eraedal/`)
- **Objective**: Audit and deepen the setting dossiers of **Eraedal**, harmonizing:
  1. The Physical Shell: Palladium Fantasy geography and mortal kingdoms (`Library/`).
  2. The Ancient Bones: Praemal / Ptolus history, subterranean horrors, and Galchutt corruption (`Library/Ptolus/`).
  3. The Active Pulse: Pathfinder 2e Remaster mechanics, ancestries, classes, and Golarion pantheon.
- **Awaiting**: Conclusion of AP distillation or user initiation of Phase 5.

---

## 🗺️ Micro-Batch Execution Schedule (27 Files / 11 Batches) — [100% COMPLETE]

| Micro-Batch | Status | Target Files | Target Directory | Focus & Theme |
| :--- | :---: | :--- | :--- | :--- |
| **MB 1** | **[COMPLETE]** | `The Eye.md`, `The Ring.md` | `01-Atlas/Absalom Station/` | Pinnacle governance dome & central commercial disc |
| **MB 2** | **[COMPLETE]** | `The Arms.md`, `The Spike.md` | `01-Atlas/Absalom Station/` | Docking ports/customs & ventral industrial core |
| **MB 3** | **[COMPLETE]** | `The Ghost Levels.md`, `The Armada.md`, `Starstone.md` | `01-Atlas/Absalom Station/` | Derelict underdecks, orbital flotilla, divine reactor/beacon |
| **MB 4** | **[COMPLETE]** | `The Plenara.md`, `The Lorespire Complex.md` | `01-Atlas/Absalom Station/` | Pact Council senate & Starfinder Society headquarters |
| **MB 5** | **[COMPLETE]** | `Bastion.md`, `The Arcanamirium.md` | `01-Atlas/Absalom Station/` | Stewards military citadel & technomancy university |
| **MB 6** | **[COMPLETE]** | `Jatembe Park.md`, `The Freemarket.md` | `01-Atlas/Absalom Station/` | Apex botanical wonderland & multi-tier trade bazaar |
| **MB 7** | **[COMPLETE]** | `Downlow.md`, `Fogtown.md` | `01-Atlas/Absalom Station/` | Slum underbelly, black markets, coolant runoff alleys |
| **MB 8** | **[COMPLETE]** | `Little Akiton.md`, `The Neon Trench.md`, `The Vesk Quarter.md` | `01-Atlas/Absalom Station/` | Immigrant warrens, cybernetic strip, reptilian martial enclaves |
| **MB 9** | **[COMPLETE]** | `Acquisitives.md`, `Dataphiles.md`, `Exo-Guardians.md` | `02-Factions/` | SFS internal factions (mercenaries, hackers, defenders) |
| **MB 10** | **[COMPLETE]** | `Wayfinders.md`, `Second Seekers.md`, `Advocates.md`, `The Master of Stars.md` | `02-Factions/` & `01-Atlas/Absalom Station/` | SFS internal factions & mobile flagship carrier |
| **MB 11** | **[COMPLETE]** | `Ysoki.md`, `Shobhads.md` | `04-Lore/Species/` | Ratfolk & four-armed giant ancestries |

---

## 🛠️ Technical Architecture & Environment Guardrails

### 1. Shell Autonomy & Guard Configuration
- **Shell-Guard Whitelist**: The global `PreToolUse` hook in `C:\Users\lelan\.gemini\config\hooks\shell-guard.js` checks for `campaign-wiki` in `args.Cwd` and `workspacePaths`, returning `{ "decision": "allow" }`.
- **Repository Authority (`AGENTS.md`)**: The agent is authorized to run direct PowerShell commands, searches (`Select-String`, `Get-ChildItem`, `git grep`), and compilation builds (`npx quartz build`) directly in `run_command` without intermediate scratch scripts.
- **Protected Actions**: Destructive git commands (`reset --hard`, `clean -fd`, `push --force`) and wholesale deletion of lore archives remain strictly forbidden without explicit user confirmation.

### 2. Quartz Content Rules & Conventions
- **Content Root**: `content/` is the sole source directory parsed by Quartz. Root-level files (`backlog.md`, `handoff.md`, `roadmap.md`, `AGENTS.md`, and `README.md`) are ignored by the site compiler and remain clean project tracking assets.
- **Wikilinks**: All links must use Obsidian/Quartz wikilink syntax: `[[Target Page]]` or `[[Target Page|Alias]]`.
- **HTML Block Warning**: Never wrap wikilinks or Markdown formatting inside raw HTML tags like `<p>` or `<div>` without blank-line separation, as CommonMark/Remark parses raw HTML blocks as literal text without converting wikilinks into hyperlinks.
- **Standard Note Schema**:
  ```markdown
  ---
  title: "Location or Faction Name"
  aliases:
    - "Common Moniker"
    - "Colloquial Epithet"
  description: "One-sentence summary for search cards and graph tooltips."
  tags:
    - location/station-sector (or location/district, faction, lore/species)
    - starfinder
    - pact-worlds
    - absalom-station
  ---

  > [!info] Quick Facts
  > **Parent Location:** [[Absalom Station]]
  > **Atmosphere / Gravity:** Standard / Artificial $\times 1$ G
  > ...
  ```

---

## 🔄 Session Recovery Protocol (In Case Chat Is Truncated or Reset)
1. Read `handoff.md` to identify the active micro-batch and current operational position.
2. Cross-reference `backlog.md` and `roadmap.md` to confirm completed vs. pending tasks.
3. Review the latest files created in `content/Worlds/Starfinder/01-Atlas/Absalom Station/`.
4. Run `npx quartz build` to ensure the compilation pipeline is 100% clean.
5. Resume immediately with the active micro-batch without losing a step.
