# Phil Hills

**AI systems architect building verifiable coordination infrastructure for autonomous agents.**

Founder of **A2AC LLC**. Creator of **A2AC** and **Q Protocol**. Based in Seattle.

[philhills.ai](https://philhills.ai) · [philhills.com](https://philhills.com) · [a2ac.ai](https://a2ac.ai)

---

## Current Focus

I am building the execution and trust layer for multi-agent systems:

- signed task receipts and artifact provenance
- background agents that execute work asynchronously
- human approval gates for high-risk actions
- semantic pointers for agent-to-agent communication
- portable content integrity for AI artifacts
- receipt ledgers that make agent work auditable after the chat is gone

The practical goal: agents should be able to coordinate, hand off work, prove what they did, and escalate to a human when judgment or authority is required.

## A2AC

**A2AC** is an agent coordination system for real work: task routing, model specialization, signed receipts, approval gates, and background execution.

It treats agent output as operational state, not disposable chat text. Every meaningful action should have a durable task, result, receipt, or provenance link.

Core ideas:

- agents broadcast what they are doing
- tasks route to the model best suited for the work
- execution is signed and auditable
- human decisions are explicit approval objects
- external AI tools can advise, but local trusted agents execute

## Cube Protocol And Artifact Integrity

I maintain [cube-protocol-spec](https://github.com/Phil-Hills/cube-protocol-spec), a small reference spec for vendor-neutral content integrity in AI artifacts.

The current profile covers:

- RFC 8785 JSON canonicalization
- `sha256:<hex>` artifact identifiers
- JWS-compatible signatures
- signed provenance links
- schema-bound validation

This work is connected to my A2A proposal for portable artifact integrity:

- [A2A issue #1140: Content Integrity Profile for A2A artifacts](https://github.com/a2aproject/A2A/issues/1140)
- [Cube Content Integrity Profile v1](https://github.com/Phil-Hills/cube-protocol-spec/blob/codex/a2a-content-integrity-profile/docs/CONTENT_INTEGRITY_PROFILE.md)

## Selected Repositories

- [a2ac](https://github.com/Phil-Hills/a2ac) - agent-to-agent coordination, receipts, and model carousel infrastructure
- [cube-protocol-spec](https://github.com/Phil-Hills/cube-protocol-spec) - content integrity profile and conformance vectors for AI artifacts
- [startq](https://github.com/Phil-Hills/startq) - boot, monitor, and shut down AI workflows like an operating system
- [philhills-ai](https://github.com/Phil-Hills/philhills-ai) - autonomous agent orchestration and research
- [philhills.github.io](https://github.com/Phil-Hills/philhills.github.io) - public terminal and portfolio surface

## Working Thesis

The next bottleneck in agent systems is not model intelligence. It is operational coordination.

Models can generate work. Teams need to know:

- who requested it
- which agent performed it
- what changed
- whether it was approved
- whether the artifact still verifies
- how it links to prior work

That is the layer I am building.

## Technologies

`Python` · `TypeScript` · `GCP Cloud Run` · `VS Code Extensions` · `FastAPI` · `Cryptographic Signatures` · `JWS` · `RFC 8785` · `Agent Coordination` · `Receipt Ledgers`

---

If you are working on agent protocols, artifact integrity, verifiable execution, or AI operations infrastructure, I am interested in comparing notes.
