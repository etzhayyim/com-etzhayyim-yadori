# yadori — DNS availability and acquisition actor

`yadori` (宿) is the standalone Tier-B actor for read-only domain availability checks and member-principal reservation intents. Canonical metadata, data, schemas, and lexicon contracts are EDN; externally served identity JSON is isolated under `wire/`.

## Layout

- `src/yadori/` — availability, reservation, social, and Murakumo logic
- `test/yadori/` — deterministic offline tests
- `schema/` and `contracts/lexicon/` — canonical EDN contracts
- `data/` — representative registrar data, seed, and identity journal
- `wire/identity/` — DID and profile JSON projections
- `docs/adr/` — actor-owned decisions and gate-gap records

Run `bb test`. Live RDAP and registrar mutations remain operator/Council gated; the repository test suite performs no outward writes.
