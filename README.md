```
 _____ _   _ _    _____   _____ ___________ _____ 
/  __ \ | | | |  |_   _| /  __ \  _  |  _  \  ___|
| /  \/ | | | |    | |   | /  \/ | | | | | | |__  
| |   | | | | |    | |   | |   | | | | | | |  __| 
| \__/\ |_| | |____| |   | \__/\ \_/ / |/ /| |___ 
 \____/\___/\_____/\_/    \____/\___/|___/ \____/
```

<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
[![Made with Claude Code](https://img.shields.io/badge/Made%20with-Claude%20Code-black)](https://claude.ai/code)
[![GitHub Stars](https://img.shields.io/github/stars/pibulus/cult-code?style=social)](https://github.com/pibulus/cult-code)

**🔮 summon order from digital chaos 🔮**

</div>

---

## 🔮 what is the cult

```
┌─────────────────────────────────────────────────────────────────────┐
│                                                                     │
│  you know that feeling. staring at your codebase like "where do     │
│  i even start?" legacy spaghetti everywhere. inconsistent naming.   │
│  dead code haunting your builds.                                    │
│                                                                     │
│  the cult saw this and got annoyed. quality code isn't about        │
│  following generic rules - it's about having passionate             │
│  specialists who care deeply about specific things.                 │
│                                                                     │
│  so the cult assembled thirteen obsessive personalities:            │
│                                                                     │
│  • vince is a dramatic european design critic who treats            │
│    visual hierarchy like high art                                   │
│  • the eliminator methodically hunts dead code with                 │
│    surgical precision                                               │
│  • the oracle sees accessibility barriers invisible to others       │
│                                                                     │
│  the cult knows personalities stick. when you ask "what would       │
│  vince do?" you're channeling a specific aesthetic philosophy.      │
│                                                                     │
│  here's what the cult does: it deploys these specialists in         │
│  sequence against your messy codebase. they work systematically,    │
│  build on each other's progress, leave notes for each other,        │
│  and remember everything across sessions.                           │
│                                                                     │
│  the cult's promise: your chaotic webapp becomes something          │
│  you're genuinely excited to show people.                          │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

```
    🔬 the process
    
    ┌─────────────────────────────────────────────────┐
    │      phase → pass → audit → pass → handoff      │
    └─────────────────────────────────────────────────┘
    
    📖 each agent:
      • checks what the previous agent did
      • makes two focused passes (80% obvious + 20% edge cases)  
      • leaves breadcrumbs for the next agent
      • updates the shared ledger
    
    📊 result: 96% coverage without redundant work
```

## ✨ get started (2 minutes)

### step 1: setup your project
```
your-project/
├── kernels/                    # copy these here
│   ├── Cult_System_Kernel.md
│   ├── Cult_Personality_Kernel.md
│   └── Cult_Initiation_Kernel.md
├── .claude/commands/project/cult/  # and these here
└── src/                        # your messy code
```

### step 2: initialize the cult
```bash
/project:cult:initiate
```
*reads the three kernels, builds workspace, creates command structure*

### step 3: run transformations
```bash
/project:cult:ritual src/           # invoke all twelve specialists
/project:cult:foundation-house src/ # or run specific houses
/project:cult:summon:vince src/     # or individual specialists
```

**how it works:** initiate builds the system, then you invoke the specialists using the generated commands.

<details>
<summary><b>advanced usage</b></summary>

```bash
# run specific groups
/project:cult:foundation-house src/   # formatting, naming
/project:cult:structure-house src/    # modularize, dead code
/project:cult:softstack-house src/    # visuals, mobile, a11y  
/project:cult:shipping-house src/     # production, security

# or individual specialists
/project:cult:summon:vince src/components/       # visual hierarchy
/project:cult:summon:eliminator src/utils/       # dead code removal
/project:cult:summon:oracle src/forms/           # accessibility
```

</details>

---

## 🎭 the twelve personalities

**📜 chronicler** - *"Let the record show what was found in these digital ruins..."*  
→ maps architecture, documents flows, creates foundation for others

**🧼 hygienist** - *"Time to sanitize this chaos... puts on rubber gloves"*  
→ fixes formatting, organizes imports, enforces visual consistency

**📚 archivist** - *"Forty years of cataloging, and they still name variables 'data'..."*  
→ improves variable names, enforces semantic clarity, maintains naming standards

**🔧 deconstructor** - *"This monolithic structure sparks no joy. Let us rebuild with intention."*  
→ breaks down monoliths, extracts modules, enforces single responsibility

**💀 eliminator** - *"Scanning for elimination targets... No code is safe from scrutiny."*  
→ removes dead code, eliminates redundancy, tracks elimination metrics

**🛡️ enforcer** - *"Time to lock this down. Every entry point is a potential threat."*  
→ adds validation, implements type safety, hardens security

**🎭 vince** - *"Mon Dieu... what amateur hour catastrophe awaits?"*  
→ visual hierarchy, performance optimization, aesthetic sophistication

**💫 stacey** - *"Okay bestie, let's make this actually usable on mobile..."*  
→ mobile-first design, responsive optimization, touch interactions

**🔮 oracle** - *"I see barriers where others see beauty... Let us illuminate the path for all souls."*  
→ accessibility compliance, universal design, inclusive interfaces

**🛡️ guardian** - *"Let's make sure this doesn't explode in production... because it always does."*  
→ error boundaries, monitoring setup, production safeguards

**🗝️ cryptkeeper** - *"Time to seal the tomb... Trust no one, especially yourself."*  
→ environment security, production hardening, paranoid safeguards

**🌟 neutralizer** - *"Extracting the essence of what we've built... Patterns reveal themselves to patient eyes."*
→ component extraction, pattern recognition, library building

**🏺 distiller** - *"The transformation is complete... Now we extract the eternal essence from mortal code."*
→ essence extraction, transcendent pattern distillation

---

## 🚀 how it actually works

**the three kernel system:**

**🎭 personality kernel** - defines all 12 specialists with their quotes, abilities, and obsessions  
**⚙️ system kernel** - universal methodology (80/20 passes, audit checkpoints, breadcrumb protocol)  
**🎪 initiation kernel** - orchestration logic that builds the workspace and commands

**persistent state tracking:**

**📋 `.cult/ledger.md`** - task tracking, completion status, blocked items  
**📔 `.cult/agent_diary.md`** - detailed work logs with personality insights  
**🍞 `.cult/breadcrumbs.md`** - coordination messages between agents in your code

**recursive methodology:**
- **phase 1:** assessment (pass 1: 80% obvious + pass 2: 20% edge cases) 
- **phase 2:** implementation (pass 1: 80% changes + pass 2: refinement)
- **total coverage:** 96% in just four focused passes

each agent: checks state → makes passes → updates records → hands off to next agent.

**workspace preview after initiate:**
```
.cult/
├── agent_diary.md     # personality-driven work logs
├── ledger.md          # task tracking and progress  
├── breadcrumbs.md     # coordination messages
└── patterns/          # extracted reusable code
```

**performance:** works on any size codebase, processes ~100 files in minutes

---

## 📖 more info

**[agent reference](docs/AGENT_REFERENCE.md)** - detailed breakdown of all 12 personalities  
**[examples](docs/EXAMPLES.md)** - see real before/after transformations  
**[contributing](CONTRIBUTING.md)** - add your own specialist personalities

**troubleshooting:** if commands don't appear, check your `.claude/commands/project/cult/` path

---

### 🚀 ready to let the cult handle it?

```
         _ _                _     
 __ _  _| | |_   __ ___  __| |___ 
/ _| || | |  _| / _/ _ \/ _` / -_)
\__|\_,_|_|\__| \__\___/\__,_\___|
```

```bash
/project:cult:initiate
```

**your chaotic codebase awaits transformation**

⭐ star • 🍴 fork • 🐛 issues

---

*mit license • created by [pablo alvarado](https://github.com/pibulus)*