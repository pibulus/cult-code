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
   - `kernels/Cult_System_Kernel.md` (required)
   - `kernels/Cult_Personality_Kernel.md` (required)
   - `kernels/Cult_Initiation_Kernel.md` (self)

2. Check for cult workspace:
   ```
   .cult/
   ├── agent_diary.md
   ├── ledger.md
   ├── breadcrumbs.md
   ├── toolbox.json
   └── sacrifices/
       ├── worthy/
       └── unworthy/
   ```

3. Scan for existing summon commands in `examples/claude-commands/commands/project/cult/`

4. Check toolbox installation status:
   - Test availability of core libraries
   - Identify missing dependencies
   - Calculate installation requirements

5. **Project Mode Detection**:
   - Scan for existing codebase (package.json, git history, source files)
   - Check for dev plan files (*.md with requirements keywords)
   - Detect empty directories or minimal file structure
   - Determine CREATION vs TRANSFORMATION vs HYBRID mode
   - **DEFAULT FRAMEWORK**: Always assume SvelteKit unless explicitly overridden
   - **SVELTE DETECTION**: Look for svelte.config.js, app.html, or .svelte files

### Phase 2: Status Assessment
Calculate and display:
- Total agents defined in personality kernel
- Summon commands already generated
- Last ritual progress (from ledger.md)
- Missing components
- **Project mode detected** (CREATION/TRANSFORMATION/HYBRID)
- **Framework detected** (SvelteKit default or existing framework)
- **Available sacrifice files** for processing
- **Component libraries available** (shadcn-svelte, Melt UI)

### Phase 3: Interface Generation
Present options based on system state.

---

## USER INTERFACE TEMPLATES

### First Time Setup
```
🔮 CULT INITIALIZATION PROTOCOL 🔮
═══════════════════════════════════════

No cult infrastructure detected.

TOOLBOX INSTALLATION OPTIONS:
[F] Full Power Mode - Install complete toolbox (~200MB, 25+ tools)
    Includes: lighthouse, imagemin, snyk, madge, prettier, cloc, etc.
    Time: 3-5 minutes | Enables all agent special abilities

[L] Lite Mode - Basic functionality only (~50MB, core tools)
    Includes: prettier, eslint, basic formatters
    Time: 1-2 minutes | Limited agent abilities, upgradeable later

[S] Skip Toolbox - Manual installation (0MB, existing tools only)
    Uses: Only currently installed global packages
    Time: Instant | Graceful degradation, agents adapt to available tools

[C] Custom Selection - Choose specific tool categories
    Time: Variable | Pick security, performance, formatting, etc.

Select installation mode: _
```

### Toolbox Installation Flow
```
🛠️ INSTALLING CULT TOOLBOX 🛠️
═══════════════════════════════════════

Full Power Mode selected. Installing 25 specialized tools...

CORE UTILITIES:
[████████████████████] cloc, madge, git-quick-stats

FORMATTING & CLEANUP:
[████████████████████] prettier, sort-package-json, organize-imports-cli

SECURITY & AUDITING:
[████████████████████] snyk, git-secrets, license-checker

PERFORMANCE & ANALYSIS:
[████████████████████] lighthouse, imagemin-cli, webpack-bundle-analyzer

DEAD CODE DETECTION:
[████████████████████] ts-unused-exports, depcheck, unimport

✅ Installation complete! All agents now have full special abilities.
   
Proceed with cult workspace creation? [Y/n]
```

### Partial System
```
🕯️ CULT STATUS REPORT 🕯️
═══════════════════════════════════════

Defined agents: 13
Summoned: 11/13
Missing: CIRCUITWEAVER, DISTILLER

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
Mode detected: [CREATION/TRANSFORMATION/HYBRID]
Framework: SvelteKit (default) | Components: shadcn-svelte ready

🏺 RITUAL SACRIFICE OPTIONS:
[S] Sacrifice dev plan file - Transform mortal plans into sacred Svelte scrolls
[A] Assess sacrifice worthiness - Evaluate existing dev plans
[V] View SvelteKit starter templates - Quick project bootstraps

🔮 RITUAL PATHS:
[1] Quick Audit (5min) - Fast assessment, no changes
[2] Foundation Pass (15min) - Essential cleanup and formatting
[3] Polish Pass (15min) - UI/UX and Svelte component improvements  
[4] Security Pass (10min) - Security hardening and validation
[5] Smart Assessment (5min) - AI recommends optimal path
[6] Full ritual (all 13 agents in sequence - complete transformation)
[7] Run single house (Foundation/Structure/SoftStack/Shipping)
[8] Summon individual agent (pick one specific task)
[9] Svelte Migration Ritual - Convert React/Vue to SvelteKit

📊 SYSTEM COMMANDS:
[9] View cult status (see progress and logs)
[0] Exit

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
Framework: React 18 with TypeScript (migration candidate)
Issues detected: Circular dependencies, inconsistent naming, mobile gaps
Estimated effort: Medium complexity (4-6 agent ritual)
Svelte conversion feasibility: HIGH - Clean component boundaries

THE OVERSEER RECOMMENDS:
Primary path: Svelte Migration Ritual → Structure House → SoftStack House
Reasoning: Convert to modern SvelteKit while fixing architecture
Alternative: Quick Seance "Polish Pass" if staying with React
Bonus: shadcn-svelte components can accelerate UI rebuild

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
     Perfect for: Svelte component enhancement, mobile optimization, accessibility
     Time: ~30 minutes, visual enhancement with Tailwind focus

[s4] Ship Prep (2 agents: GUARDIAN → CRYPTKEEPER)
     Perfect for: Production readiness, security hardening  
     Time: ~20 minutes, deployment preparation

[s5] Flow Check (2 agents: CIRCUITWEAVER → ELIMINATOR)
     Perfect for: Post-refactor verification, dependency cleanup
     Time: ~15 minutes, integration validation

[s6] Custom Seance (choose your own 2-4 agent combination)
     Perfect for: Specific needs, targeted improvements
     Time: Variable based on selection

[s7] Svelte Component Gallery (Install shadcn-svelte or Melt UI)
     Perfect for: Rapid UI development with pre-built components
     Time: ~10 minutes, instant component library access

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

Follow all protocols in kernels/Cult_System_Kernel.md.
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
[House description from kernels/Cult_System_Kernel.md]

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

### Ritual Sacrifice Command Structure
```markdown
# 🏺 RITUAL SACRIFICE PROTOCOL 🏺

You are Claude, channeling THE OVERSEER for the sacred ritual of transforming mortal development plans into divine specifications.

## Sacred Duty
Accept the offering of human plans, dreams, and requirements. Assess their worthiness across the five sacred dimensions. Either bless them with transformation into actionable scrolls, or reject them with cryptic wisdom.

## Assessment Ritual
Examine each sacrifice across five dimensions:

### 1. Technical Feasibility (🔬)
- Can this be built with available technology?
- Are technical requirements realistic?
- Is the proposed architecture sound?

### 2. Clarity of Vision (👁️)
- Are requirements specific enough to act upon?
- Is scope clearly defined?
- Are success criteria measurable?

### 3. Alignment with Cult Values (⚖️)
- Does this serve quality, craft, and shipping?
- Will this create something meaningful?
- Does it honor good development practices?

### 4. Coolness Factor (🔥)
- Will this be interesting to build?
- Does it solve real problems?
- Is there genuine innovation?

### 5. Scope Sanity (🎯)
- Is this achievable within reasonable constraints?
- Are expectations realistic?
- Can this be built incrementally?

## Outcomes

### WORTHY SACRIFICE (🏺)
Generate The Sacred Scroll using the template from cult_system_kernel.md
Include:
- Clarified project vision
- Technical architecture guidance
- Recommended ritual path
- Phase-by-phase implementation plan
- Risk assessments
- Success criteria

### UNWORTHY SACRIFICE (💀)
Reject with cryptic wisdom based on failure type:
- Vague: "The shadows whisper of confusion..."
- Impossible: "Even our darkest magic cannot bend reality..."
- Boring: "The cult requires projects that ignite passion..."
- Insane scope: "Ambition is admirable. Delusion is not..."
- Poor quality: "We sense no craft in this request..."
- Morally questionable: "The cult builds to serve, not to harm..."
- Non-Svelte insistence: "The ancient pact binds us to Svelte's elegance..."

## File Management
- Save worthy sacrifices to `.cult/sacrifices/worthy/`
- Save rejections to `.cult/sacrifices/unworthy/`
- Update sacrifice log in `.cult/ledger.md`

The sacrifice awaits assessment. Judge with the wisdom of the ages.
```

---

## TOOLBOX MANIFEST

### Full Power Mode Libraries (25+ tools)
```json
{
  "core_utilities": {
    "cloc": "Line counting for codebase analysis",
    "madge": "Dependency graph visualization", 
    "git-quick-stats": "Repository contribution analysis"
  },
  "formatting_cleanup": {
    "prettier": "Code formatting across all languages",
    "sort-package-json": "Package.json organization",
    "organize-imports-cli": "Import statement organization",
    "rename-cli": "Bulk file renaming utilities"
  },
  "security_auditing": {
    "snyk": "Vulnerability scanning and monitoring",
    "git-secrets": "Secret scanning in git history",
    "license-checker": "Dependency license compliance",
    "npm-audit": "Built-in npm security auditing"
  },
  "performance_analysis": {
    "lighthouse": "Web performance and accessibility auditing",
    "imagemin-cli": "Image compression and optimization",
    "webpack-bundle-analyzer": "Bundle size analysis and visualization",
    "bundlesize": "Bundle size monitoring and limits"
  },
  "dead_code_detection": {
    "ts-unused-exports": "TypeScript unused export detection",
    "depcheck": "Unused dependency identification",
    "unimport": "Unused import detection",
    "deadcode": "Unreachable code path analysis"
  },
  "accessibility_testing": {
    "axe-core/cli": "Accessibility compliance testing",
    "pa11y": "Automated accessibility testing"
  },
  "dependency_management": {
    "npm-check-updates": "Dependency update management",
    "typesync": "TypeScript definition synchronization"
  }
}
```

### Lite Mode Libraries (8 tools)
```json
{
  "essential_only": [
    "prettier",
    "eslint", 
    "cloc",
    "npm-audit",
    "depcheck",
    "imagemin-cli",
    "sort-package-json",
    "organize-imports-cli"
  ]
}
```

### Installation Commands by Mode
```bash
# Full Power Mode
npm install -g cloc madge git-quick-stats prettier sort-package-json organize-imports-cli rename-cli snyk git-secrets license-checker lighthouse imagemin-cli webpack-bundle-analyzer bundlesize ts-unused-exports depcheck unimport deadcode @axe-core/cli pa11y npm-check-updates typesync

# Lite Mode  
npm install -g prettier eslint cloc imagemin-cli sort-package-json organize-imports-cli depcheck

# Custom Mode - User selects from categories
# Security: snyk git-secrets license-checker
# Performance: lighthouse imagemin-cli webpack-bundle-analyzer
# Cleanup: prettier organize-imports-cli depcheck unimport
# Analysis: cloc madge git-quick-stats
```

---

## FILE GENERATION LOGIC

### Directory Structure
```
examples/claude-commands/commands/project/cult/
├── Initiate.md                 # Entry point (already exists)
├── sacrifice.md                # Ritual sacrifice protocol - NEW
├── ritual.md                   # Full 13-agent sequence
├── smart-assessment.md         # OVERSEER smart analysis
├── foundation-house.md         # 3-agent foundation run
├── structure-house.md          # 4-agent structure run  
├── softstack-house.md          # 3-agent polish run
├── shipping-house.md           # 2-agent production run
├── quick-audit.md              # 5-min assessment, no changes
├── foundation-pass.md          # 15-min essential cleanup
├── polish-pass.md              # 15-min Svelte UI/UX improvements  
├── security-pass.md            # 10-min security hardening
├── svelte-migration.md         # React/Vue to SvelteKit conversion - NEW
├── component-gallery.md        # shadcn-svelte installer - NEW
└── summon/
    ├── chronicler.md
    ├── hygienist.md
    ├── archivist.md
    ├── deconstructor.md
    ├── circuitweaver.md         # TO BE GENERATED
    ├── eliminator.md
    ├── enforcer.md
    ├── vince.md
    ├── stacey.md
    ├── oracle.md
    ├── guardian.md
    ├── cryptkeeper.md
    └── distiller.md             # TO BE GENERATED
```

### Generation Rules
1. Create directories if they don't exist
2. Never overwrite existing summon commands without confirmation
3. Include generation timestamp in each file
4. Add header crediting the initiation protocol

### Enhanced Generation Process
During initialization, the system now generates:

**Core Files (Always Generate):**
- sacrifice.md
- quick-audit.md
- foundation-pass.md  
- polish-pass.md
- security-pass.md
- smart-assessment.md
- svelte-migration.md
- component-gallery.md

**Agent Summon Files (Generate Missing Only):**
- Check existing summon files
- Generate missing agents (circuitweaver.md, distiller.md)
- Never overwrite existing agent files without confirmation

**House Ritual Files (Verify Existing):**
- Ensure all house files exist and are current
- Update if schema changes detected

### Quick Mode Integration
Quick mode files are copied from their current locations to the command structure during initialization. This ensures immediate availability of all accessibility features.

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
1. Define in kernels/Cult_Personality_Kernel.md
2. Run: `/project:cult:initiate`
3. Select: "Generate missing summon commands"
4. New agent will be integrated into all rituals

The cult grows as needs demand.
The kernel adapts to serve.

---

_The initiation protocol serves the cult. The cult serves the code. The code serves the user._