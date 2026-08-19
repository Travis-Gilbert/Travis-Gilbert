

## Theorem

An agent harness. Typed memory that persists across sessions, coordination that lets multiple coding agents (Claude Code, Codex) work the same repository through shared state instead of stepping on each other, and 60+ MCP tools in production. CommonPlace is the knowledge surface it pairs with; together they form the full harness.

Underneath sits **RustyRed**, a multi-model database written in Rust, over 100 crates in the working monorepo: a property-graph core with vector, lexical, and spatial retrieval, a relational query planner, and git-style versioning of graph state. Commit the graph, diff it, branch it, merge it. Fork an agent's memory the way you fork a repo. It speaks the Postgres wire protocol and Redis RESP, so existing clients connect without a new driver.

Measured, not asserted: on a 20,000-node / 40,000-edge graph it sustains roughly 8,300 node upserts per second and answers Personalized PageRank in 27 ms median, full round trip, reproducible from a one-command harness.

A trimmed standalone release is public under MIT, with a live read-only instance you can point an agent at.

[RustyRed GraphDB](https://github.com/Travis-Gilbert/RustyRed-Graph-Database) · [one-click deploy](https://railway.com/new/template/rustyred-graphdb)

The learned layer is **Theseus**: GNN and knowledge-graph-embedding enrichment, learned rerankers, reinforcement-learning tool selection, and graph-fused language models trained with LoRA on rented GPUs. The graph reasons. The LLM expresses.

[Graph-fused Gemma 31B image](https://github.com/users/Travis-Gilbert/packages/container/package/theseus-gemma-31b-glfusion)

## Also built

**our-civic-atlas**: a geospatial planning app. Track a set of keys or a multimillion dollar infrastructure project on the same map.

**RustyWeb**: search, scrape, and aggregation in Rust, built on DATAWAVE. Connects to RustyRed, Valkey, and Postgres, and composes to the shape of whatever workflow it feeds.

## Day job

Designed, built, and operate a production Django/PostGIS/GraphQL/Next.js compliance platform for a county land bank: a fifteen-thousand-parcel portfolio with roughly eight hundred properties active in inspection workflows, six platforms collapsed into one operating surface, and automated weekly reporting.

## Stack

Rust (tokio, axum) · Python (Django, PyTorch) · TypeScript (Next.js) · PostgreSQL/PostGIS · Tauri · SwiftUI

Deploys on Railway. Trains on RunPod.

## Contact

Open to ML systems, backend engineering, and agent infrastructure work. If you have an interesting computer science problem outside those, send it anyway.

[travisgilbert.me](https://travisgilbert.me) · 1travisgilbert@gmail.com
