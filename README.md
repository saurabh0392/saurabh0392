# Hi, I'm Saurabh 👋

Senior Solutions Architect at Amazon Shipping. Before that, nearly a decade across product and engineering, most recently as a Staff PM at Shippo building developer APIs and AI systems for logistics. I build things out of curiosity, mostly AI tools, and I like owning a bet end to end, from the market thesis down to prototyping it myself.

📍 New York, NY  ·  [saurabhsharan.dev](https://saurabhsharan.dev)  ·  [LinkedIn](https://www.linkedin.com/in/saurabhsharan/)  ·  saurabhsharan03@gmail.com

---

## What I'm building

Two AI products built independently. ctx is finished and open source. The Gaffer is in active development, source private for now.

### ctx: a context layer for AI coding agents (finished, open source)
ctx shows what a coding agent's context actually costs, then reclaims noisy tool output with a byte-for-byte way back. It started with a question about my own AI bill: 77,000 tokens of tool definitions rode along on every request. Partway in I found my safety metric could not have detected a failure, so I invalidated the claim and rebuilt the product around evidence you can check on your own sessions.

- An itemized Context Bill built from your real sessions, not benchmarks
- Trims gate on randomized comparisons of your own work, and every trim can be rewound byte for byte
- Local by default: no account, no background telemetry

The project is done, deliberately. The full story, pivot included: [saurabhsharan.dev](https://saurabhsharan.dev)

Install: `brew install saurabh0392/ctx/ctx` or `cargo install ctx-agent` · [Source, MIT](https://github.com/saurabh0392/ctx)

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

## Writing

[AI Inversion: Make the Model Ask the Questions](https://saurabhsharan.dev/writing/ai-inversion) (Nov 2026). For documents whose value lies in the decisions inside them, I stopped letting the model write. It asks the questions and I make each call.

---

## Background

Senior Solutions Architect at **Amazon Shipping** since November 2026.

Before that, Staff Product Manager at **Shippo** (2022–2026), where I owned the Carrier Integrations domain: reusable platform components with engineering so integrations shipped faster and broke less, and carrier, customer, and geography bets with GTM. Highlights:
- Built and shipped an agentic AI platform (retrieval over carrier specs and codebase, served to non-engineers via Slack) that cut on-call engineering hours by 40%.
- Drove $3M+ in new GPV by leading the launch of 15+ shipping integrations.
- Scaled carrier coverage 15x, from 68 to 1000+.

Earlier: Technical PM at INECTA (Food ERP) and Software Engineer at IBM. NYU Master's in Management Information Systems.

---

## Toolbox

**Product:** Strategy & vision, 0 to 1 and 1 to 10, roadmapping, prototyping
**AI / ML:** Agentic AI, retrieval and vector search, LLM integration (local and hosted), human-in-the-loop design, evaluation and behavioral measurement
**Build:** Rust, TypeScript, Node.js, React, Python, SQL, AWS, Unity (C#)
