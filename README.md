# arknetz-registry-0f

ArkNetzWebWeaver registry shard `0f` (MIT) — one of 16 hash
shards. Holds only its slice of the global domain registry, keyed by the
first hex digit of SHA256(domain).

- `registry.json.zst` — canonical shard file (Zstd-compressed JSON; live empty state:
  `{}`, 15 bytes). `registry.json` is the plain mirror committed
  alongside it on every claim.
- `.github/workflows/register.yml` — the REGISTER-issue claim flow for
  this shard.

Live state: empty. No domains are registered in this shard yet — an empty
registry is the live starting state, not test data. The first REGISTER claim
processed by `.github/workflows/register.yml` appends the first entry here.
