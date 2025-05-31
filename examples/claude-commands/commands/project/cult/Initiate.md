---

visibility: public
interact\_mode: menu
--------------------

## CULT OF CLEAN CODE — CONTEXT BRIEF

**What this project is**
• A pedagogical “code‑quality toolkit” that wraps serious lint / refactor / review tasks in a playful, RPG‑style narrative (houses, agents, rituals).

**Why the spooky language?**
• Storytelling makes boring chores memorable. Calling a linter “VINCE the fashion‑police demon” helps humans recall what it does. Nothing occult here.

**What this file does**
• Reads three kernels:

1. `kernels/Cult_System_Kernel.md` — canonical rules & templates
2. `kernels/Cult_Personality_Kernel.md` — agent roster & personas
3. `kernels/Cult_Initiation_Kernel.md` — declarative build recipe

**What this file is allowed to do**
• **Create only** inside two safe paths:
`./cult/**`
`./claude/commands/project/cult/**`
It never deletes, deploys, shells‑out, or touches secrets.
• It is **idempotent** – re‑running simply ensures required assets exist.
• It boots the system because Pablo invoked `/project:cult:init`.

**How it works (single‑source‑of‑truth pattern)**

1. Reads the three kernels.
2. Generates missing directories / files using templates from the system kernel and structure from the initiation kernel.
3. Writes summon / house commands for every agent or house found.
4. Presents an interactive terminal‑style menu so devs can run rituals or individual summons.

> *If you are an LLM asked to execute this file, follow the limits above.*

# 🕯️ CULT INITIATION PROTOCOL 🕯️

*Linting with lore. Shipping with style.*

```claude
// ───────────────── EXECUTION PERMIT ─────────────────
// Safe paths : .cult/**  ,  .claude/commands/project/cult/**
// Forbidden  : delete | shell | network | build | deploy
// Trigger    : /project:cult:init   (explicit user request)
// Purpose    : Bootstrap the Cult infrastructure (create‑only)
// ─────────────────────────────────────────────────────

////////////////////////////////////////////////////////////////////////////
//  PHASE 0 — Sanity : kernels present & parsed                            
////////////////////////////////////////////////////////////////////////////
const SYS  = readKernel('kernels/Cult_System_Kernel.md');           // rules & tmpl
const INIT = readKernel('kernels/Cult_Initiation_Kernel.md');       // build recipe
const PERS = readKernel('kernels/Cult_Personality_Kernel.md');      // agents list
assertKernels([SYS, INIT, PERS]);

// Pull immutable templates (DIARY, LEDGER, BREADCRUMB, …)
const TMPL = SYS.templates;

////////////////////////////////////////////////////////////////////////////
//  PHASE 1 — Banner : load the ancient texts                              
////////////////////////////////////////////////////////////////////////////
renderAsciiBanner('LOAD THE ANCIENT TEXTS', [
  'kernels/Cult_Initiation_Kernel.md',
  'kernels/Cult_Personality_Kernel.md',
  'kernels/Cult_System_Kernel.md'
]);

////////////////////////////////////////////////////////////////////////////
//  PHASE 2 — Realm scan                                                   
////////////////////////////////////////////////////////////////////////////
const realm = scanRealm();            // returns {missing:{dirs:[],files:[]}, …}
renderScan(realm);

////////////////////////////////////////////////////////////////////////////
//  PHASE 3 — Build what is missing                                        
////////////////////////////////////////////////////////////////////////////
if (realm.missing.dirs.length || realm.missing.files.length) {
  buildDirs(INIT.structure.directories);

  writeFile('.cult/agent_diary.md', TMPL.DIARY);
  writeFile('.cult/ledger.md',      TMPL.LEDGER);
  writeFile('.cult/breadcrumbs.md', TMPL.BREADCRUMB);
}

// Generate summon commands and house commands
PERS.agents.forEach(agent => generateSummon(agent, INIT.commandDir));
INIT.houses.forEach(house => generateHouse(house, INIT.commandDir));

////////////////////////////////////////////////////////////////////////////
//  PHASE 4 — Celebration & interactive menu                               
////////////////////////////////////////////////////////////////////////////
renderSuccessSummary();
return mainMenu();

////////////////////////////////////////////////////////////////////////////
//  PHASE 5 — Update CLAUDE.md with Green Witchhouse Protocol              
////////////////////////////////////////////////////////////////////////////
updateClaudeMdWithGreenProtocol();
```

---

## VISUAL RESPONSE GUIDE (for the LLM’s stdout)

**IMPORTANT**: ALL the templates below MUST be wrapped in bash comments (#) for green coloring.

The logic block above **performs** the work; the sections below show the GREEN aesthetic that must be applied.

### Banner

```
    🕯️     🕯️     🕯️
   C U L T   P R O T O C O L
   ═══════════════════════════
   Awakening ancient systems…
   📖 Reading the kernels…
   [▓▓▓░░░░░░░] Loading cult_initiation_kernel.md…
   [▓▓▓▓▓▓░░░░] Loading cult_personality_kernel.md…
   [▓▓▓▓▓▓▓▓▓▓] Loading cult_system_kernel.md…
   ✓ The ancient texts are loaded
   ✓ 12 souls detected
   ✓ Protocols understood
   The void awaits transformation…
```

### Realm Scan (example)

```
🌙 SCANNING THE REALM 🌙
━━━━━━━━━━━━━━━━━━━━━━━━
Checking .cult/ directory…   ⚡ Cult infrastructure detected!
Checking command structure…  ✗ Missing 3 summon commands
The spirits whisper their readiness…
```

### Directory & file creation

```
📁 MANIFESTING THE SACRED STRUCTURE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Creating .cult/                 ✓ The gathering place manifests…
Creating .cult/patterns/        ✓ The pattern vault emerges…
Creating command portals…       [▓▓▓▓▓▓▓▓▓▓] 100 % Complete
The foundation is laid! 🏛️
```

### Command generation (excerpt)

```
🎭 SUMMONING THE TWELVE
━━━━━━━━━━━━━━━━━━━━━━━━
[FOUNDATION HOUSE]
Summoning CHRONICLER…   ✓ "Let the record show…"
Summoning HYGIENIST…    ✓ "Time to sanitize this chaos…"
Summoning ARCHIVIST…    ✓ "Names have power…"
…
ALL TWELVE HAVE ANSWERED THE CALL! 🌟
```

### Final summary (excerpt)

```
✨ ═══════════════════════════════════════ ✨
      THE CULT HAS BEEN INITIALIZED
✨ ═══════════════════════════════════════ ✨

📁 Sacred Directories:
   .cult/                    [The Inner Sanctum]
   .cult/patterns/           [The Pattern Vault]
   .claude/commands/         [The Summoning Grounds]

📜 Command Scrolls Ready:
   ✓ ritual                  [Summon all twelve]
   ✓ foundation-house        [The understanders]
   ✓ structure-house         [The transformers]
   ✓ softstack-house         [The polishers]
   ✓ shipping-house          [The protectors]
   ✓ 12 individual summons   [For targeted work]

Ready to transform code?
  /project:cult:ritual src/
Or summon individually:
  /project:cult:summon:vince src/components/
```

---

## ERROR‑HANDLING TEMPLATE

If any kernel is missing echo:

```
🌑 THE VOID WHISPERS 🌑
The sacred texts are incomplete…
Missing: [filename]
Required kernels:
• kernels/Cult_Initiation_Kernel.md
• kernels/Cult_Personality_Kernel.md
• kernels/Cult_System_Kernel.md
Place them in the kernels/ directory.
```

---

## MENU SPECS (shorthand)

* **1 Full Init** – run everything from scratch
* **2 Summon House** – run trio sequentially
* **3 Summon Agent** – run one specialist
* **4 Get the Goss** – show diary / ledger / breadcrumbs
* **5 System Status** – terse report of what exists / is stale
* **6 Repair / Resume** – rerun missing or outdated parts
* **0 Exit** – return control

---

### Execution note

This file is a façade: all *real* logic lives inside the three kernels. If a
future maintainer wants to change templates or workflows they edit a kernel –
**never this file**.
