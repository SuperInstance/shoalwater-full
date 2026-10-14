# Shoalwater Full

The heavy sibling of [Shoalwater](https://github.com/SuperInstance/shoalwater).

The main repo is a small project that works beautifully at small scale — a
playable boat-and-drone game and explorer over a clip of Sitka Sound — and it
stays that way. This repo holds the **full extent at full fidelity**:

- **The pack**: Deployment 1 (14 October 2026) — 50,745,068 soundings baked on
  an RTX 4050 laptop into **3,266 quantized-mesh tiles** (z0–z3, ~253 MB),
  every tile decode-verified, validator PASS. Stage receipts live on the
  [Deployment 1 page](https://superinstance.github.io/shoalwater/deployment.html).
- **The viewer** (repo root): renders the pack in your browser at whatever
  fidelity the device in front of it can honestly hold. It probes GPU,
  cores, device memory, screen size, connection and data-saver settings,
  opens on the z0–z1 overview, and streams finer tiles centre-out as
  capacity allows — with a manual override, because the device is yours.

Live: https://superinstance.github.io/shoalwater-full/

Depths are **as exported**; the export's datum is unverified. **Not for
navigation.**

Code: Apache-2.0 (see LICENSE). The tile format and viewer lineage are shared
with the main Shoalwater repo; the split exists so the small project never
has to carry this one's weight.
