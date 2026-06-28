# Hi, I'm Saurabh 👋

Staff Technical Product Manager building B2B SaaS and developer-API products, with a focus on self-serve growth, usage-based monetization, and AI systems that automate real work. Nearly a decade across product and engineering. I like owning a bet end to end, from the market thesis down to prototyping it myself.

📍 Indianapolis, IN  ·  [LinkedIn](https://www.linkedin.com/in/saurabhsharan/)  ·  saurabhsharan03@gmail.com

---

## What I'm building

Two AI products I am developing independently. These are early and the source is private, so what follows is the what, the direction, and how I validate the work, not the internals.

### ctx: a self-learning context layer for AI coding agents
ctx is a trust layer for AI coding agents (Claude Code and Cursor). Most tools compress an agent's context to save tokens and hope nothing breaks. ctx takes the opposite stance: it proves a context change is safe from your own behavior before it makes one, and stays fail-closed until it has that proof. Your original tool output always stays in the transcript.

- **Proof before action:** ctx learns from how you actually work and only changes what it can show, from your own data, will not cost you accuracy.
- **A measurement layer, not a guesser:** it treats real outcomes as the source of truth instead of synthetic benchmarks, and will not act on a signal it has not earned.
- **Cross-agent:** it understands sessions across more than one agent, so it can tell when the agent's own context handling, rather than your prompt, caused a problem.
- **Experiment-driven:** continuous, automated A/B testing and a dashboard that shows cost per task and where the wins actually come from.

**Direction:** from a personal tool today toward a shared "context truth" layer that scores whether your agents' context decisions are costing you corrections, across agents, and acts only on what it can prove.

**Validation:** the whole system is built on production behavioral outcomes as ground truth, with deliberate honesty gates. It holds back from claiming a win until your own data clears a real bar, and refuses to publish headline numbers it cannot stand behind.

*Stack: Rust, SQLite, embedded dashboard.*

### The Gaffer: a conversation-first football management sim
The Gaffer reimagines football management by replacing the menus of a game like Football Manager with real natural-language conversation. You talk to your assistant, your players, the press, and the board, and every decision ripples across the season through a consequence engine. Every significant choice is a conversation, and every conversation is remembered.

Three layers working together:
- **Simulation:** a custom match engine, a spatial simulation of all 22 players with real ball physics and role-aware movement.
- **Narrative AI:** a multi-stage local-LLM pipeline that turns each thing you say into bounded, validated consequences and in-character replies, blending larger and smaller models for cost and latency.
- **Render:** a Unity 6 HDRP 3D match view with a broadcast camera, wrapped in an Electron and React desktop shell.

**What makes it feel real:** the same words land differently depending on who you say them to and how you say it, characters carry memory and their own agendas, and decisions compound over weeks instead of resetting. The hard part, and where most of the design work lives, is making consequences feel earned rather than random.

**Direction:** toward a full 38-game season across every part of the job, with emergent unscripted situations and a voice layer.

**Validation:** dozens of deterministic engine selftests, a consequence model checked against real-world football incidents, an agent play-test loop that drives the game end to end and files structured bug reports, and heavy frame-by-frame iteration on movement and cinematic quality. Around 3,800 players and 124 clubs seeded.

*Stack: TypeScript, Node.js, React, Electron, Unity 6 HDRP (C#), local LLMs via Ollama, graph and vector stores.*

---

## Background

Currently Staff Product Manager at **Shippo**, where I own the Address & Tracking API. Highlights:
- Built and shipped an agentic AI platform (retrieval over carrier specs and codebase, served to non-engineers via Slack) that cut on-call engineering hours by 40%.
- Drove $3M+ in new GPV by leading the launch of 15+ shipping integrations.
- Scaled carrier coverage 15x, from 68 to 1000+.

Earlier: Technical PM at INECTA (Food ERP) and Software Engineer at IBM. NYU Master's in Management Information Systems.

---

## Toolbox

**Product:** Strategy & vision, 0 to 1 and 1 to 10, roadmapping, prototyping
**AI / ML:** Agentic AI, retrieval and vector search, LLM integration (local and hosted), human-in-the-loop design, evaluation and behavioral measurement
**Build:** Rust, TypeScript, Node.js, React, Python, SQL, Unity (C#)
