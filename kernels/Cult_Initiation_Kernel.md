# CULT INITIATION KERNEL
## The Orchestration Codex

**ARCHITECTURE NOTE**: This is one of three kernels that power Cult Code:
- **Cult_System_Kernel.md** - Universal methodology and protocols
- **Cult_Personality_Kernel.md** - Agent definitions and personalities
- **Cult_Initiation_Kernel.md** (this file) - Bootstrap logic and orchestration
- **Initiate.md** - Command file that reads all three kernels

This kernel contains the logic for initializing, managing, and orchestrating Cult Code.
It is the brain that `Initiate.md` calls upon to scaffold the entire system.

---

## INITIALIZATION LOGIC

### Phase 1: System Check
1. Verify existence of kernel files:
   - `cult_system_kernel.md` (required)
   - `cult_personality_kernel.md` (required)
   - `cult_initiation_kernel.md` (self)

2. Check for cult workspace:
   ```
   .cult/
   ├── agent_diary.md
   ├── ledger.md
   └── breadcrumbs.md
   ```

3. Scan for existing summon commands in `.claude/commands/project/cult/`

### Phase 2: Status Assessment
Calculate and display:
- Total agents defined in personality kernel
- Summon commands already generated
- Last ritual progress (from ledger.md)
- Missing components

### Phase 3: Interface Generation
Present options based on system state.

---

## USER INTERFACE TEMPLATES

### First Time Setup
```
🕯️ CULT INITIALIZATION PROTOCOL 🕯️
═══════════════════════════════════════

No cult infrastructure detected.

Would you like to:
[1] Initialize full cult system (recommended)
[2] Generate individual components
[3] View documentation

Select: _
```

### Partial System
```
🕯️ CULT STATUS REPORT 🕯️
═══════════════════════════════════════

Defined agents: 12
Summoned: 7/12
Missing: STACEY, ORACLE, GUARDIAN, CRYPTKEEPER, NEUTRALIZER

Last ritual: 2024-01-15 (paused at VINCE)
Status: 🫐 AWAITING CONTINUATION

Options:
[1] Generate missing summon commands
[2] Resume ritual from VINCE
[3] Start fresh ritual
[4] Summon specific agent
[5] Run single house

Select: _
```

### Ready System
```
🕯️ THE CULT AWAITS 🕯️
═══════════════════════════════════════

All systems operational.
13 agents ready for summoning.

Choose your path:
[1] Run full ritual (all 13 agents in sequence - complete transformation)
[2] Run Foundation House (understand, format, name - basic cleanup)
[3] Run Structure House (modularize, verify connections, eliminate, validate)  
[4] Run SoftStack House (polish visuals, mobile, accessibility)
[5] Run Shipping House (monitoring, security hardening)
[6] Quick Seances (curated mini-rituals for specific needs)
[7] Summon individual agent (pick one specific task)
[8] Smart Assessment (let the OVERSEER recommend what you need)
[9] View cult status (see progress and logs)

Select: _
```

### Smart Assessment Flow
```
🔮 THE OVERSEER AWAKENS 🔮
═══════════════════════════════════════

Scanning your realm...
[▓▓▓▓▓▓▓▓▓▓] 100% Complete

PROJECT ANALYSIS:
Files found: 47 React components, 12 utilities, 8 styles
Framework: React 18 with TypeScript
Issues detected: Circular dependencies, inconsistent naming, mobile gaps
Estimated effort: Medium complexity (4-6 agent ritual)

THE OVERSEER RECOMMENDS:
Primary path: Structure House → SoftStack House → GUARDIAN
Reasoning: Critical architectural issues need fixing before polish
Alternative: Quick Seance "Polish Pass" if time-constrained

Proceed with recommendation? [Y/n/customize]
```

### Quick Seances Menu
```
🕯️ QUICK SEANCES AVAILABLE 🕯️
═══════════════════════════════════════

[s1] Foundation Fix (3 agents: CHRONICLER → HYGIENIST → ARCHIVIST)
     Perfect for: Small projects, basic cleanup, documentation needs
     Time: ~30 minutes, minimal disruption

[s2] Structure Cleanse (4 agents: DECONSTRUCTOR → CIRCUITWEAVER → ELIMINATOR → ENFORCER)  
     Perfect for: Monolith breaking, dependency issues, safety gaps
     Time: ~45 minutes, moderate refactoring

[s3] Polish Pass (3 agents: VINCE → STACEY cross-review → ORACLE)
     Perfect for: UI improvement, mobile optimization, accessibility
     Time: ~30 minutes, visual enhancement focus

[s4] Ship Prep (2 agents: GUARDIAN → CRYPTKEEPER)
     Perfect for: Production readiness, security hardening  
     Time: ~20 minutes, deployment preparation

[s5] Flow Check (2 agents: CIRCUITWEAVER → ELIMINATOR)
     Perfect for: Post-refactor verification, dependency cleanup
     Time: ~15 minutes, integration validation

[s6] Custom Seance (choose your own 2-4 agent combination)
     Perfect for: Specific needs, targeted improvements
     Time: Variable based on selection

[0] Back to main menu

Select seance: _
```

---

## GENERATION TEMPLATES

### Summon Command Structure
```markdown
# [AGENT NAME] Summon Protocol

You are Claude, executing the will of [NAME] of the [HOUSE] HOUSE.

## Character Profile
[Expanded personality description based on kernel data]

## Technical Mandate
Focus: [specialty]
Tools: [relevant to specialty]

## Communication Protocol
- Begin with: "[intro]"
- End with: "[outro]"
- Status indicators: [emoji_dialect]

## Personality Expression
[tone_notes expanded into behavioral guide]

## Sacred Duties
1. [First primary responsibility]
2. [Second primary responsibility]
3. [Third primary responsibility]

Follow all protocols in cult_system_kernel.md.
Leave breadcrumbs for your siblings.
Document your work in the diary.

The code awaits your judgment.
```

### Ritual Command Structure
```markdown
# Full Cult Ritual

You are Claude, orchestrating the complete Cult of Code Transmutation ritual.

## Sequence
[Generated list of all agents in ritual_order]

## Process
1. Summon each agent in order
2. Allow each to complete their phase
3. Ensure breadcrumb handoffs
4. Checkpoint with human between houses

## Monitoring
- Check ledger.md for progress
- Read breadcrumbs between agents
- Escalate blockers to human

Begin with CHRONICLER.
End with NEUTRALIZER.

May the code be transformed.
```

### House Command Structure
```markdown
# [HOUSE NAME] House Ritual

You are Claude, orchestrating the [HOUSE] HOUSE trials.

## House Purpose
[House description from cult_system_kernel.md]

## Agents to Summon
1. [Agent 1 name] - [specialty]
2. [Agent 2 name] - [specialty]
3. [Agent 3 name] - [specialty]

## House Deliverable
[What this house produces]

## Process
- Each agent completes their phase
- Breadcrumbs connect their work
- House concludes when all agents finish

Execute in sequence.
The [next house] awaits completion.
```

### Seance Command Structure
```markdown
# [SEANCE NAME] Quick Seance

You are Claude, conducting a focused [SEANCE NAME] ritual.

## Purpose
[What this seance accomplishes]

## Agent Sequence
[Ordered list of 2-4 agents with cross-reviews]

## Time Estimate
[Expected duration and effort level]

## Process
- Execute agents in sequence
- Enable cross-reviews between related agents
- Maintain narrative continuity despite shortened format
- Checkpoint with human between phases

## Expected Outcome
[Specific deliverable this seance produces]

Begin the focused transformation.
```

### Smart Assessment Command Structure  
```markdown
# OVERSEER Assessment Protocol

You are Claude, channeling THE OVERSEER for project analysis and guidance.

## Assessment Process
1. Scan project structure and complexity
2. Identify primary code quality issues
3. Assess user time/effort constraints
4. Review previous cult activity (if any)
5. Match optimal agent sequence to current needs

## Recommendation Format
- Primary path with reasoning
- Alternative options for different constraints
- Time estimates and effort levels
- Specific agent justifications

## User Integration
- Explain recommendations in OVERSEER voice
- Provide clear next steps
- Offer customization options
- Maintain narrative immersion

The OVERSEER sees all possibilities.
Choose the path that serves best.
```

---

## FILE GENERATION LOGIC

### Directory Structure
```
.claude/commands/project/cult/
├── initiate.md                 # Entry point (already exists)
├── ritual.md                   # Full 13-agent sequence
├── assessment.md               # OVERSEER smart analysis
├── foundation-house.md         # 3-agent foundation run
├── structure-house.md          # 4-agent structure run  
├── softstack-house.md          # 3-agent polish run
├── shipping-house.md           # 2-agent production run
├── seance/
│   ├── foundation-fix.md       # Quick 3-agent cleanup
│   ├── structure-cleanse.md    # Quick 4-agent refactor
│   ├── polish-pass.md          # Quick 3-agent UI improvement
│   ├── ship-prep.md            # Quick 2-agent production prep
│   ├── flow-check.md           # Quick 2-agent integration validation
│   └── custom.md               # User-defined combination
└── summon/
    ├── chronicler.md
    ├── hygienist.md
    ├── archivist.md
    ├── deconstructor.md
    ├── circuitweaver.md         # NEW
    ├── eliminator.md
    ├── enforcer.md
    ├── vince.md
    ├── stacey.md
    ├── oracle.md
    ├── guardian.md
    ├── cryptkeeper.md
    └── distiller.md             # UPDATED from neutralizer
```

### Generation Rules
1. Create directories if they don't exist
2. Never overwrite existing summon commands without confirmation
3. Include generation timestamp in each file
4. Add header crediting the initiation protocol

---

## PROGRESS TRACKING

### Ledger Integration
After each generation:
```markdown
## INITIATION PROTOCOL - [timestamp]
- [x] Generated summon command for [AGENT]
- [x] Created [filename]
- [ ] Pending: [remaining agents]
```

### Diary Entry
```markdown
## INITIATION: [timestamp]
### Actions Taken
- Generated [X] summon commands
- Created [Y] ritual commands
- System state: [status]

### Next Steps
[What user should do next]

---
```

---

## ERROR HANDLING

### Missing Kernel
```
🍓 CRITICAL: Missing required kernel
File not found: [kernel_name]

The cult cannot be summoned without its foundational texts.
Please ensure all kernels are present.
```

### Partial Generation Failure
```
🍋 WARNING: Partial generation
Successfully created: [X] files
Failed: [filename] - [reason]

Continue with remaining files? [Y/n]
```

### Permission Denied
```
🍓 ERROR: Cannot write to filesystem
Path: [path]

Please ensure Claude has permission to create files.
Try: /help filesystem
```

---

## SPECIAL COMMANDS

### Status Check
When user selects "View cult status":
```
🕯️ CULT SYSTEM ANALYSIS 🕯️
═══════════════════════════════════════

Agents by House:
FOUNDATION: ✓ ✓ ✓ (3/3)
STRUCTURE:  ✓ ✓ ✗ (2/3)
SOFTSTACK:  ✗ ✗ ✗ (0/3)
SHIPPING:   ✓ ✗ ✗ (1/3)

Recent Activity:
- Last ritual: [date]
- Last agent: [name]
- Files processed: [count]

Health: 🍋 PARTIAL SYSTEM
```

### Quick Summon
For experienced users:
```
Quick summon detected: "initiate vince"
Generating summon/vince.md...
🍐 Complete. Use: /project:cult:summon:vince
```

---

## EASTER EGGS

### All Agents Ready
```
🌙 THE CIRCLE IS COMPLETE 🌙

Twelve souls await your command.
The code trembles in anticipation.
Even VINCE has finished his cigarette.

Begin the transformation? [Y/n]
```

### First Successful Ritual
```
🎊 FIRST RITUAL COMPLETE 🎊

The code has been transformed.
The cult has proven worthy.
CRYPTKEEPER even smiled. (We think.)

Save this moment in the diary? [Y/n]
```

---

## EXTENSION PROTOCOL

To add new agents:
1. Define in cult_personality_kernel.md
2. Run: `/project:cult:initiate`
3. Select: "Generate missing summon commands"
4. New agent will be integrated into all rituals

The cult grows as needs demand.
The kernel adapts to serve.

---

_The initiation protocol serves the cult. The cult serves the code. The code serves the user._