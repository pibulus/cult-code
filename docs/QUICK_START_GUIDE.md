# 🚀 CULT CODE QUICK START GUIDE

*Get your first code transformation in 5 minutes*

---

## 🎯 Your First Ritual

### Step 1: Initialize the Cult
```bash
/project:cult:initiate
```

**What happens:** The cult creates its workspace and generates all 12 agent summon commands.

**You'll see:**
```
🕯️ CULT INITIALIZATION PROTOCOL 🕯️
✓ The ancient texts are loaded
✓ 12 souls detected
✓ Protocols understood
📁 Sacred Directories created
📜 Command Scrolls Ready
```

### Step 2: Pick Your Starting Point

**New to the cult?** Start with Foundation House:
```bash
/project:cult:foundation-house src/
```

**Want the full experience?** Run the complete ritual:
```bash
/project:cult:ritual src/
```

**Have a specific problem?** Summon the right specialist:
```bash
/project:cult:summon:vince src/components/     # Visual issues
/project:cult:summon:eliminator src/utils/    # Dead code cleanup
```

### Step 3: Watch the Magic

Each agent will:
1. **Check the ledger** for previous work
2. **Review the diary** for context  
3. **Scan for breadcrumbs** left by other agents
4. **Execute their specialty** in systematic passes
5. **Document their work** for the next agent

---

## 🎭 Meet Your First Three Agents

### THE CHRONICLER 📜
*"Let the record show what was found..."*

**What they do:** Maps your codebase like an archaeologist
- Documents all functions and components
- Creates flow diagrams for complex logic
- Builds the foundation map for everyone else

**When to summon:** Starting any new project work, unclear codebase architecture

### THE HYGIENIST 🧼  
*"Time to sanitize this chaos..."*

**What they do:** Obsessively cleans formatting
- Fixes indentation and spacing inconsistencies
- Organizes imports alphabetically
- Standardizes quote styles and brackets

**When to summon:** Code looks messy, inconsistent formatting, pre-review cleanup

### THE ARCHIVIST 📚
*"What fresh naming hell is this?"*

**What they do:** Grudgingly improves terrible names
- Replaces ambiguous variable names
- Enforces consistent naming conventions
- Documents naming decisions

**When to summon:** Confusing variable names, inconsistent naming patterns

---

## 📋 What You'll See During Work

### Agent Status Updates
```
🔍 THE CHRONICLER - Phase 1, Pass 1
Scanning src/components for undocumented functions...
Found 12 unnamed functions, 3 complex flows
Creating documentation scaffolds...

📜 PASS: Documentation foundation established
Moving to Pass 2 for edge cases...
```

### Breadcrumb Trail
Agents leave comments in your code:
```javascript
<!-- CHRONICLER-P1-S3: HANDOFF @HYGIENIST Formatting inconsistent -->
<!-- HYGIENIST-P2-S8: COMPLETE All formatting standardized -->
export const processUserData = (userData) => {
  return userData.map(item => item.value)
}
```

### State Tracking
Check progress anytime:
```bash
# View work logs
cat .cult/agent_diary.md

# Check task status  
cat .cult/ledger.md

# See agent communications
cat .cult/breadcrumbs.md
```

---

## 🎯 First Run Expectations

### Foundation House (~15-30 minutes)
- **CHRONICLER**: Documents your codebase structure
- **HYGIENIST**: Cleans up formatting inconsistencies  
- **ARCHIVIST**: Improves variable and function names

**Result:** Clean, documented, semantically clear foundation

### Common First-Time Experiences

**"THE CHRONICLER found a lot of undocumented functions"**  
✅ Normal! Most codebases have documentation gaps. The Chronicler maps everything first.

**"THE HYGIENIST changed a lot of formatting"**  
✅ Expected! Consistent formatting is the foundation for everything else.

**"THE ARCHIVIST complained about my variable names"**  
✅ They complain about everyone's names. The improvements make code much clearer.

---

## 🚨 When Things Go Wrong

### Agent Gets Stuck
```bash
# Check what they were working on
cat .cult/agent_diary.md

# Look for error breadcrumbs in code
grep -r "ERROR" src/

# Resume from ledger status
cat .cult/ledger.md
```

### Unexpected Changes
- **All changes are documented** in the diary
- **Breadcrumbs explain reasoning** in code comments
- **Ledger shows progress** and blockers

### Want to Undo
Agents don't automatically commit changes. Use your normal git workflow:
```bash
git diff                    # See what changed
git checkout -- src/       # Undo changes
git add . && git commit     # Keep changes
```

---

## 🎪 Advanced First Steps

### Target Specific Issues
```bash
# Visual hierarchy problems
/project:cult:summon:vince src/components/

# Mobile responsiveness  
/project:cult:summon:stacey src/

# Dead code cleanup
/project:cult:summon:eliminator src/utils/

# Security hardening
/project:cult:summon:enforcer src/api/
```

### Resume Interrupted Work
The cult automatically detects incomplete work:
```
🕯️ CULT STATUS REPORT 🕯️
Last ritual: paused at VINCE
Status: 🫐 AWAITING CONTINUATION

[2] Resume ritual from VINCE
```

### Monitor Progress
```bash
# Quick status check
/project:cult:status

# Detailed progress
cat .cult/ledger.md | grep -E "\\[x\\]|\\[ \\]"
```

---

## 🎯 Success Indicators

### You're Getting Value When:
- **Agent personalities feel distinct** (VINCE's drama vs ELIMINATOR's efficiency)
- **Work builds systematically** (each agent references previous work)
- **Quality improves measurably** (cleaner code, better performance, fewer bugs)
- **You start thinking in agent terms** ("This needs VINCE" or "ELIMINATOR would hate this")

### Ready for More When:
- Foundation House completes successfully
- You understand the diary/ledger/breadcrumb system
- You can summon individual agents confidently
- You want to try Structure House or full ritual

---

## 🎭 Next Steps

1. **Complete Foundation House** on a real project
2. **Read the agent outputs** in diary and breadcrumbs
3. **Try individual agent summons** for specific problems
4. **Run Structure House** for architectural improvements
5. **Experience the full ritual** for complete transformation

Remember: The cult serves the code. The code serves the user.

*May your first transformation be swift and systematic.* 🕯️✨