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
- **Critical Pacing Rule**:
  > [!IMPORTANT]
  > **"No more than one file at a time so I have a chance to keep up :-)"**
  > Always generate or edit exactly **one major lore file per turn**, verify it with Quartz, provide a structured summary, and await user confirmation before proceeding to the next.

---

## 📍 Current Progress & Immediate Next Step

### Current Position: Phase 1 Complete (14 of 14 Bodies Chronicled & Verified)
1. **[[Mataras]] (The Sun)** — Complete & verified.
2. **[[Aballon]] (The Horse / The Forge)** — Complete & verified.
3. **[[Castrovel]] (The Green Mother)** — Complete & verified.
4. **[[Absalom Station]] (The Nexus at the Void)** — Complete & verified.
5. **[[Akiton]] (The Red Planet)** — Complete & verified.
6. **[[Verces]] (The Ring of Nations)** — Complete & verified.
7. **[[The Diaspora]] (The Shattered Belt)** — Complete & verified.
8. **[[The Idari]] (The Eternal Colony Ship)** — Complete & verified.
9. **[[Eox]] (The Dead World)** — Complete & verified.
10. **[[Triaxus]] (The Wanderer)** — Complete & verified.
11. **[[Liavara]] (The Dreamer)** — Complete & verified.
12. **[[Bretheda]] (The Cradle)** — Complete & verified.
13. **[[Apostae]] (The Maiden)** — Complete & verified.
14. **[[Aucturn]] (The Stranger)** — Complete & verified.

### 🎯 Immediate Next Step: Phase 2 — Interplanetary Factions & Power Blocs
- **Target File**: `content/Worlds/Starfinder/02-Factions/Pact Council.md`
- **Entity**: **[[Pact Council]] (The Directorate of the Absalom Pact)**
- **Key Lore Elements to Incorporate**:
  - Foundational history: The ratification of the **Absalom Pact** in **291 AG** in response to the devastating Veskarium invasion.
  - Structure & Chambers: The bicameral parliament meeting in the Plenara on [[Absalom Station]]—the **Delegation** (representing member worlds and protectorates) and the **Directorate** (the executive directorate council led by Prime Executive Kumara Melacruz).
  - Voting dynamics: Representation of worlds, corporate lobbying (AbadarCorp), the uneasy votes of Eox and Apostae, and veto thresholds.
  - Jurisdictions & Enforcement: Pact-wide civil rights, economic trade standards, military mobilization authority, and relationship with [[The Stewards]].

----

## 🛠️ Technical Architecture & Environment Guardrails

### 1. Shell Autonomy & Guard Configuration
- **Shell-Guard Whitelist**: The global `PreToolUse` hook in `C:\Users\lelan\.gemini\config\hooks\shell-guard.js` has been patched to check for `campaign-wiki` in `args.Cwd` and `workspacePaths`, returning `{ "decision": "allow" }`.
- **Repository Authority (`AGENTS.md`)**: The agent is authorized to run direct PowerShell commands, searches (`Select-String`, `Get-ChildItem`, `git grep`), and compilation builds (`npx quartz build`) directly in `run_command` without needing intermediate scratch `.ps1` scripts.
- **Protected Actions**: Destructive git commands (`reset --hard`, `clean -fd`, `push --force`) and wholesale deletion of lore archives remain strictly forbidden without explicit user confirmation.

### 2. Quartz Content Rules & Conventions
- **Content Root**: `content/` is the sole source directory parsed by Quartz. Root-level files (such as `backlog.md`, `handoff.md`, `roadmap.md`, `AGENTS.md`, and `README.md`) are ignored by the site compiler and remain clean project tracking assets.
- **Wikilinks**: All links must use Obsidian/Quartz wikilink syntax: `[[Target Page]]` or `[[Target Page|Alias]]`.
- **HTML Block Warning**: Never wrap wikilinks or Markdown formatting inside raw HTML tags like `<p>` or `<div>` without blank-line separation, as CommonMark/Remark parses raw HTML blocks as literal text without converting wikilinks into hyperlinks.
- **Standard Note Schema**:
  ```markdown
  ---
  title: "World or Location Name"
  aliases:
    - "Common Moniker"
    - "Archaic Epithet"
  description: "One-sentence summary for search cards and metadata."
  tags:
    - location/planet (or location/station, location/star)
    - starfinder
    - pact-worlds
    - atlas/celestial-body
  ---

  > [!info] Quick Facts
  > **System:** [[Mataras System]] (The [[Pact Worlds]])
  > **Orbital Position:** ...
  > **Planetary Diameter:** $\times 1$ Terrestrial
  > **Surface Gravity:** $\times 1$ Standard Gravity
  > ...
  ```

### 3. Build & Verification Protocol
After writing or updating any lore note in `content/`, always run:
```bash
npx quartz build
```
Verify that the compilation emits all files cleanly without errors.
