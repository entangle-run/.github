# Entangle

Entangle is a self-hosted federated runtime for observable coding-agent
organizations.

It models an AI engineering organization as a graph:

- agents, human users, and services are nodes;
- edges define allowed communication, delegation, review, and approval;
- runners execute assigned nodes wherever they live;
- User Nodes sign their own tasks, replies, approvals, and reviews;
- Nostr carries signed coordination events;
- git-backed references carry durable artifacts and source changes;
- Studio and CLI expose the same Host-owned projection.

The goal is not to build another chatbot wrapper or a hidden orchestrator. The
goal is to make coding agents and human participants operate as a governed,
inspectable, distributed organization.

## Repositories

- [`entangle`](https://github.com/entangle-run/entangle) — runtime monorepo:
  Host, runner, Studio, CLI, User Client, shared contracts, deployment tooling,
  deterministic smoke paths, and architecture records.
- [`entangle-website`](https://github.com/entangle-run/entangle-website) —
  public website, docs, and notes.
- [`.github`](https://github.com/entangle-run/.github) — organization profile
  and default community health files.

## Current Status

Entangle is pre-release. The runtime has deterministic proofs for the core
federated path: Host, relay, runners, User Node runtime, fake OpenCode/model
execution, projection, Studio, CLI, memory, approvals, source-change evidence,
and git-backed artifact handoff.

Real OpenCode/provider credentials, real coding tasks with commits or pull
requests, physical multi-machine deployment, and production security hardening
remain explicit validation work.

## Product Rule

A compact developer deployment may run several nodes on one machine with a
local relay and local git service. That must not create local-only product
assumptions. The same identity, assignment, signed-message, artifact, and
projection model should work when the parts live on different machines.

## Links

- Website: <https://entangle.run>
- Runtime: <https://github.com/entangle-run/entangle>
- Website source: <https://github.com/entangle-run/entangle-website>

## License

Entangle projects are open source under the Apache License 2.0 unless a
repository states otherwise.
