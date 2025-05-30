# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Cult Code is a narrative-driven code quality toolkit that transforms routine linting, refactoring, and review tasks into an engaging, RPG-style experience. The system uses 12 specialized "agent" personalities organized into 4 "houses" to systematically improve codebases through focused, memorable interventions.

## Core Architecture

### Three-Kernel System
The entire system is built on three foundational markdown files:

1. **`kernels/Cult_System_Kernel.md`** - Universal methodology, protocols, and operational rules
2. **`kernels/Cult_Personality_Kernel.md`** - Definitions of all 12 agent personalities with their specialties
3. **`kernels/Cult_Initiation_Kernel.md`** - Orchestration logic and command generation templates

### The Twelve Agents
Organized into four sequential houses:

**Foundation House** (understanding):
- CHRONICLER - Documentation and flow mapping
- HYGIENIST - Formatting and code cleanliness  
- ARCHIVIST - Naming conventions and semantic clarity

**Structure House** (rebuilding):
- DECONSTRUCTOR - Modularization and component extraction
- CIRCUITWEAVER - Data flow validation and dependency integrity
- ELIMINATOR - Dead code removal and redundancy termination
- ENFORCER - Validation, type safety, and defensive coding

**SoftStack House** (polishing):
- VINCE - Visual hierarchy and performance optimization
- STACEY - Responsive design and mobile optimization
- ORACLE - Accessibility and inclusive design

**Shipping House** (production readiness):
- GUARDIAN - Error boundaries and monitoring setup
- CRYPTKEEPER - Environment configuration and production sealing

**Transcendent Realm**:
- THE DISTILLER - Pattern extraction and library creation

### Persistent State System
The system maintains state across sessions through:

- **`.cult/ledger.md`** - Task tracking and completion status
- **`.cult/agent_diary.md`** - Detailed work logs with personality insights
- **`.cult/breadcrumbs.md`** - Coordination messages between agents in code

## Command Structure

### Initialization
- `/project:cult:initiate` - Bootstrap the entire Cult system from kernels

### Ritual Commands
- `/project:cult:ritual [path]` - Full 12-agent transformation sequence
- `/project:cult:foundation-house [path]` - Foundation house only (3 agents)
- `/project:cult:structure-house [path]` - Structure house only (4 agents)
- `/project:cult:softstack-house [path]` - SoftStack house only (3 agents)
- `/project:cult:shipping-house [path]` - Shipping house only (2 agents)

### Individual Agent Summons
- `/project:cult:summon:[agent_name] [path]` - Invoke specific agent
- Examples: `/project:cult:summon:vince src/components/`

## Working with the System

### Before Making Changes
1. Always check if kernels need to be read to understand current agent definitions
2. Review existing `.cult/` directory for state information
3. The system is designed to be **additive only** - it creates but never deletes

### Development Workflow
1. Use `initiate` to bootstrap the system
2. Run specific houses or agents based on current needs
3. Each agent follows a standardized methodology: `PHASE → PASS → STEP → AUDIT`
4. Agents leave breadcrumbs for coordination and handoff

### File Safety
The system is designed with strict safety protocols:
- Only creates files in `.cult/` and `.claude/commands/project/cult/` directories
- Never deletes, deploys, shells out, or touches secrets
- All operations are idempotent - safe to re-run

## Key Principles

### Universal Methodology
Every agent follows the same process:
1. **Pre-Work**: Check ledger → Review diary → Scan breadcrumbs → Define scope
2. **Phase 1**: Assessment (80% obvious issues → Audit → 20% edge cases → Audit)
3. **Phase 2**: Implementation (80% changes → Audit → Refinement → Audit)
4. **Post-Work**: Update diary → Update ledger → Leave breadcrumbs → Handoff

### Personality-Driven Quality
Rather than generic "improve this code" prompts, each agent has:
- Specific technical expertise and focus areas
- Memorable personality traits and communication styles
- Clear rules about what they must/never do
- Awareness of other agents they coordinate with

### State Persistence
The system maintains memory across sessions through structured logging and breadcrumb protocols, enabling compound intelligence over time.

## Important Files and Locations

- `kernels/` - Core system definitions (read-only reference)
- `examples/claude-commands/` - Example command structure and templates
- `docs/` - Additional documentation and references
- `.cult/` - Working directory created during initialization
- `.claude/commands/project/cult/` - Generated command files

## Usage Notes

- The system works on any size codebase and processes ~100 files in minutes
- Each agent is designed to handle specific aspects of code quality
- The narrative framework makes quality standards memorable and actionable
- All changes follow a review-before-commit workflow with human approval points