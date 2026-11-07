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
