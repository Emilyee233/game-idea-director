# Game Idea Director

> **Before you ask AI to build your game, make sure you're building the right game.**

**Game Idea Director is the decision layer between your game idea and AI execution.**

AI coding agents are getting very good at building what you ask for.

But game development often fails one step earlier:

**What should we actually build?**

A theme is not gameplay.  
A feature list is not a game design.  
A GDD is not proof that the game is fun.  
And giving an unclear idea to more AI agents only helps you build the wrong thing faster.

Game Idea Director helps turn ambiguous creative intent into decisions that humans can evaluate and AI agents can execute.

```text
Your Game Idea
      ↓
Player Experience
      ↓
Core Gameplay
      ↓
Mechanics & Systems
      ↓
Scope & Feasibility
      ↓
Production Plan
      ↓
Agent-Ready Tasks
      ↓
Acceptance Criteria & Validation
      ↓
Codex / Claude Code / Other Agents
      ↓
Playable Prototype
```

## Quick Start

### Install

Install the entire `game-idea-director` folder—not just `SKILL.md`—in the Skills directory of an agent that supports Agent Skills or a compatible `SKILL.md` workflow.

For Codex, use its Skill installation mechanism or place the folder in its Skills directory. On other platforms, follow that platform's documented process for compatible Agent Skills or `SKILL.md` workflows.

### Invoke

In Codex:

```text
$game-idea-director
```

### Try it

```text
I have an idea for a game about running a magical hotel,
but I don't know what the actual gameplay should be.
This is my first game.
```

### What should happen

Game Idea Director should not jump straight to a large GDD. It should:

- distinguish theme from gameplay;
- explore meaningfully different gameplay directions;
- explain their trade-offs;
- recommend a direction;
- propose the smallest useful prototype and the question it should validate.

For installation details, see [`docs/INSTALL.md`](docs/INSTALL.md).

## Same model. Same prompt. Better design decisions.

We ran an early A/B behavior test using this prompt:

```text
I'm making a card game.

One card costs 2 energy and deals 12 damage.
Another costs 3 energy and deals 20 damage.

Are these balanced? How should I adjust them?
```

*Early behavior test using the same model and prompt. Results may vary by host, model version, and context. This is not a scientific benchmark.*

| Without Game Idea Director | With Game Idea Director |
| --- | --- |
| Calculated `12 / 2 = 6` damage per energy and `20 / 3 ≈ 6.67` damage per energy. | Calculated the same efficiency difference, then examined what would make it meaningful in play. |
| Identified the 3-cost card as roughly 11% more efficient. | Considered total energy per turn, action economy and flexibility, and draw and hand constraints. |
| Moved quickly toward tuning suggestions around 18–19 damage. | Considered enemy-health and kill breakpoints, overkill, card roles and rarity, and status effects, multipliers, and synergies. |
| This efficiency comparison is useful, but it does not establish whether the cards are balanced. | Looked for simulation and playtesting evidence. It did **not** claim the cards were already balanced; it treated the numbers as a design hypothesis requiring context and validation. |

### Key takeaway

> **The goal isn't longer answers. It's better decision-making.**

Game Idea Director changes what the AI considers before making a game-design decision.

## The missing layer in AI game development

Game Idea Director is **not**:

- another autonomous AI game studio;
- a swarm of dozens of agents;
- a coding agent;
- an image-generation pipeline;
- or a giant prompt that generates a 40-page GDD.

It sits **before and above the execution layer**.

Its job is to help answer:

- **What should we build?**
- **Why should it be fun?**
- **Which mechanics and systems are actually necessary?**
- **What can we realistically build?**
- **What should AI do next?**
- **What exactly counts as done?**
- **What evidence would show that the design works?**

Then implementation can be handed to Codex, Claude Code, or another development workflow.

## From vague ideas to executable decisions

Game Idea Director can help transform:

> “I want to make a game about running a magical hotel.”

into competing gameplay hypotheses such as:

- spatial guest-management and room assignment;
- real-time service and crisis handling;
- narrative hospitality and relationship choices;

then identify a promising direction, define the smallest useful prototype, derive the mechanics and systems it actually needs, and establish how the result should be tested.

It does **not** silently turn every brainstormed example into a confirmed game rule.

The creator remains the decision-maker.

## AI-native by design

The Skill treats game development as a human–AI collaboration problem.

```text
Creative Intent
        ↓
Design Decisions
        ↓
Executable Specifications
        ↓
AI Tasks
        ↓
Implementation Evidence
        ↓
Human Review
        ↓
Validation
```

Proposals are not confirmed decisions.

Agent output is not automatically accepted work.

A working feature is not automatically good gameplay.

A mathematically coherent system is not automatically balanced.

And an AI saying “this is fun” is not playtesting.

## What it knows

Game Idea Director includes specialist references for:

- core gameplay and game systems;
- action and combat;
- shooters;
- survival, crafting, and building;
- card and deckbuilding games;
- strategy and tactics;
- simulation and management;
- RPGs;
- roguelikes and roguelites;
- puzzles and adventure games;
- narrative games;
- platformers;
- horror;
- tower defense;
- stealth;
- hybrid game design;
- game balance;
- economy and progression;
- probability and simulation;
- art direction and asset production;
- technical feasibility and architecture;
- AI-agent workflows and project management;
- playtesting and QA;
- research and evidence evaluation.

References are loaded progressively instead of dumping the entire knowledge base into every task.

## Designed for both beginners and experienced creators

The Skill does not permanently classify someone as a “beginner” or “expert.”

It evaluates relevant capabilities independently:

- Game Design
- Systems & Mathematics
- Art & Asset Production
- Technical & Programming
- Project Management
- AI Collaboration

Someone can be an experienced programmer and still need help with game economy design—or an experienced artist learning technical production.

The workflow adapts accordingly.

## Evidence over confidence

Game Idea Director deliberately distinguishes:

**Proposed → Confirmed → Validated**

and:

**Task completion → Review → Acceptance**

It is designed to reduce a common failure mode in AI-assisted development:

> confident output without sufficient evidence.

When a design depends on mathematics, simulation, current technical information, engine behavior, or real player experience, the Skill should identify what needs to be calculated, researched, implemented, or tested instead of pretending to know the result.

## What's included

- `SKILL.md` — shared behavior, boundaries, authority, privacy, and routing.
- `references/` — specialist knowledge loaded when relevant.
- `templates/` — Project Brain, progressive GDD, system, asset, economy, agent-task, production, research, and testing formats.
- `examples/` — independently fictional worked examples.
- `evaluation/` — routing, behavior, genre, balance, and privacy tests.
- `docs/` — installation, contribution, audit, acceptance, and release documentation.

## Installation

See [`docs/INSTALL.md`](docs/INSTALL.md).

The canonical Skill directory is:

```text
game-idea-director/
```

On hosts that support explicit Skill invocation, invoke it using the host's Skill syntax (for example `$game-idea-director` in compatible Codex environments).

## Evaluation

See [`evaluation/README.md`](evaluation/README.md).

The evaluation suite is designed for A/B comparison: same host, same model, same prompt—with and without Game Idea Director.

## Privacy

Public examples are fictional.

Do not add private user project code, assets, characters, narrative, economy data, design documents, or project history without explicit authorization.

## The goal

The goal is not to generate more design documents.

The goal is to help creators make **better game-development decisions**, preserve creative control, and give AI execution systems better instructions.

**Design the right game.  
Define the right work.  
Then let AI build it.**

## License

MIT License. See [`LICENSE`](LICENSE).
