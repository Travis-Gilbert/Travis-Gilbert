Travis Gilbert

I just really like infrastructure.

## Theorem
An agent harness. Typed memory that persists across sessions, coordination that lets multiple coding agents (Claude Code, Codex) work the same repository through shared state instead of stepping on each other, and 60+ MCP tools in production. CommonPlace is the knowledge surface it pairs with; together they form the full harness.

Underneath sits RustyRed, a multi-model database written in Rust across 65+ crates: a property-graph core with vector, lexical, and spatial retrieval, a relational query planner, and git-style versioning of graph state. Commit the graph, diff it, branch it, merge it. Fork an agent's memory the way you fork a repo.

The learned layer is Theseus: GNN and knowledge-graph-embedding enrichment, learned rerankers, reinforcement-learning tool selection, and graph-fused language models trained with LoRA on rented GPUs. The graph reasons. The LLM expresses.

##Also built:

### our-civic-atlas: 
A geospactial planning app. Never forget where you put your keys or run a multimillion dollar infrastructure project.
### RustyWeb: 
web search, scrape, aggregate, built from Rust and Datawave connects to the RustyRed database, Redis (Valkey), Postgres. Very modular set up according to your workflow.
### Markdown-theory
Markdown, computationally beautiful.

Day job: designed, built, and operate a production Django/PostGIS compliance platform for a county land bank, tracking roughly 15,000 properties through inspection workflows
travisgilbert.me


## Tech Stack
Rust (tokio, axum), Python (Django, PyTorch), TypeScript (Next.js), PostgreSQL/PostGIS, Tauri, SwiftUI. Deploys on Railway. Trains on RunPod.

### Contact

Open to contract work on agent infrastructure, ML systems, and backend engineering. 1travisgilbert@gmail.com
<!--
**Travis-Gilbert/Travis-Gilbert** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
