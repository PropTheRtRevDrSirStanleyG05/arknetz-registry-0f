# arknetz-registry-0f

ArkNetzWebWeaver registry shard `0f` (MIT) — one of 16 hash
shards. Holds only its slice of the global domain registry, keyed by the
first hex digit of SHA256(domain).

- `registry.json.zst` — canonical shard file (Zstd-compressed JSON; empty
  seed: `{}`, 15 bytes). `registry.json` is the plain mirror committed
  alongside it on every claim.
- `.github/workflows/register.yml` — the REGISTER-issue claim flow for
  this shard.

Seed state (2026-11-20): empty. No domains are registered yet — this is test
seed data, no real user content.
