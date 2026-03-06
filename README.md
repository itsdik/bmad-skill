# BMAD Method — Claude Code Skill

**Breakthrough Method for Agile AI-Driven Development** (v6) — a structured 4-phase methodology for building software with AI agents. Includes 9 specialized agent skills that coordinate through phases: Analysis, Planning, Solutioning, and Implementation.

## What It Does

BMAD provides a full software development lifecycle managed by specialized AI agents:

| Agent | Role | Command |
|-------|------|---------|
| **BMad Master** | Orchestrator — routes to workflows, tracks progress | `/workflow-init`, `/workflow-status` |
| **Business Analyst** | Research, brainstorming, product briefs | `/product-brief`, `/brainstorm`, `/research` |
| **Product Manager** | PRDs and technical specifications | `/prd`, `/tech-spec` |
| **System Architect** | Architecture design, solutioning gate checks | `/architecture`, `/solutioning-gate-check` |
| **UX Designer** | UX design workflows | `/create-ux-design` |
| **Scrum Master** | Sprint planning, story creation | `/sprint-planning`, `/create-story` |
| **Developer** | Story implementation, code review | `/dev-story` |
| **Builder** | Create custom workflows and agents | `/create-workflow`, `/create-agent` |
| **Creative Intelligence** | Research and creative brainstorming | `/research`, `/brainstorm` |

### Project Levels

- **Level 0:** Single atomic change (1 story)
- **Level 1:** Small feature (1-10 stories)
- **Level 2:** Medium feature set (5-15 stories)
- **Level 3:** Complex integration (12-40 stories)
- **Level 4:** Enterprise expansion (40+ stories)

## Install

### One-liner

```bash
git clone https://github.com/itsdik/bmad-skill.git ~/.claude/skills/bmad
```

### Claude Code agent install

If your Claude Code agent is installing this for you, it should:

```bash
# 1. Clone into the skills directory
git clone https://github.com/itsdik/bmad-skill.git ~/.claude/skills/bmad

# 2. Verify installation
ls ~/.claude/skills/bmad/core/bmad-master/SKILL.md
ls ~/.claude/skills/bmad/bmm/pm/SKILL.md
```

The skills are automatically available on the next Claude Code session — no further configuration needed. Claude Code discovers skills by scanning `~/.claude/skills/**/SKILL.md`.

### Manual install

1. Download or clone this repo
2. Place the contents at `~/.claude/skills/bmad/`
3. Restart Claude Code

## File Structure

```
~/.claude/skills/bmad/
├── core/
│   └── bmad-master/SKILL.md       # Orchestrator
├── bmm/                            # BMAD Method Modules
│   ├── analyst/SKILL.md            # Business Analyst
│   ├── architect/SKILL.md          # System Architect
│   ├── developer/SKILL.md          # Developer
│   ├── pm/SKILL.md                 # Product Manager
│   ├── scrum-master/SKILL.md       # Scrum Master
│   └── ux-designer/SKILL.md        # UX Designer
├── bmb/                            # BMAD Method Builders
│   └── builder/SKILL.md            # Workflow/Agent Builder
└── cis/                            # Creative Intelligence
    └── creative-intelligence/SKILL.md
```

## Quick Start

After installation, start with:

```
/workflow-init
```

This initializes BMAD in your current project and recommends the next step based on your project's size and complexity.

Check progress anytime with:

```
/workflow-status
```

## Usage Examples

```
# Initialize BMAD in your project
/workflow-init

# Create a product requirements document
/prd

# Design the architecture
/architecture

# Plan your sprint
/sprint-planning

# Create and implement a story
/create-story
/dev-story
```

## License

MIT
