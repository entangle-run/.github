# Contributing

Entangle is pre-release and the architecture is still being hardened. Changes
should keep the product model coherent:

- Entangle is the product, not a local-only runtime.
- Host, runner, User Node, operator, git principal, and engine identities must
  remain separate.
- Studio is the operator control room.
- User Client is the participant surface for a running User Node.
- CLI should use the same Host-owned boundaries as Studio and User Client.
- Messages coordinate work; artifacts preserve work products.
- Deterministic tests should cover runtime behavior before claims are made.

Before opening a pull request:

1. Read the relevant docs in the target repository.
2. Keep docs and code aligned.
3. Run the checks listed by that repository.
4. Avoid public claims that require live-provider or physical multi-machine
   validation unless that validation was actually performed.
