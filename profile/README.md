## HAVEN — Reclaiming the Internet for the User.

We build open-source infrastructure where data stays encrypted and platforms don't hold the keys. No centralized backends, no gatekeepers, no data silos.

Ownership is the only password. Media is encrypted on the publisher's machine, indexed on public networks, and unlocked only by what a reader already holds.

Docs: [https://haven-hvn.github.io/docs/](https://haven-hvn.github.io/docs/)

### 📈 Trending

[![vlm-engine PyPI Downloads](https://img.shields.io/badge/downloads-2k_/month-blue)](https://pypistats.org/packages/vlm-engine)

*[vlm-engine](https://github.com/Haven-hvn/haven-vlm-engine-package)* is gaining traction — over 2,000 downloads per month on PyPI.

### 🚀 The Stack

**Read** - `haven-dapp`

Repo: [Haven-hvn/haven-dapp](https://github.com/Haven-hvn/haven-dapp)

Site: [https://haven.pinme.dev](https://haven.pinme.dev)

Your Videos, Decentralized. Sovereign media protocol — no accounts, no passwords, your wallet is your identity and key. Open Library, stream from IPFS anywhere, decrypt fully in-browser via haven-aol VetKD gates. Includes Publish a Drip wizard + Upcoming Video Drops: each release splits into 1–10 chunks that stay locked until its mint.club bonding-curve market cap hits that chunk's target, then that chunk's key derives. Static build pinned to IPFS, offline-first cache, batch V3 unlock.

**Write** - `haven-cli`

Repo: [Haven-hvn/haven-cli](https://github.com/Haven-hvn/haven-cli)

The only surface that encrypts. Decentralized archival and automation that runs on your own machine — no hosted queue, no shared DB. Ingest → Analyze (VLM) → Encrypt (AOL) → Upload (Synapse/Filecoin) → Sync (Arkiv). Local SQLite, cron scheduling, plugin system.

**Own** - `haven-aol`

Repo: [Haven-hvn/haven-aol](https://github.com/Haven-hvn/haven-aol)

Canister smart contract: [gny6k-fqaaa-aaaab-ag3ra-cai](https://dashboard.internetcomputer.org/canister/gny6k-fqaaa-aaaab-ag3ra-cai)

The foundation. True ownership requires privacy — without it, data is just public property. ICP canister verifies an EIP-712 `GateRequest`, checks `balanceOf` via EVM RPC, then derives the key via VetKD. Only you decide who gets in.

- v1 per-file (`accessol_v1`), v3 corpus + 30-day epoch (`accessol_v3`, one derivation unlocks a whole collection, approval-cached)
- v4 market-cap-gated drip (`accessol_v4`): `SHA-256(chain:token:threshold:epoch:marketCapTarget)`. Bond curve is the only price source, 5-min cap cache, fails closed with `MarketCapNotReached` / `InvalidOracle`
- Portable Ed25519 attestations for provable holding without re-deriving


**Synthesize** - `haven-vlm-engine`

Repo: [haven-vlm-engine-package](https://github.com/Haven-hvn/haven-vlm-engine-package)

AI-powered media understanding. Verify what's inside a file without opening it — generate tags, extract metadata, and build trust in shared archives without exposing data to a corporate API. Remote OpenAI-compatible VLM, CPU-only friendly, multiplexer load-balancing with failover. Powers `haven-cli analyze`.

**Automate** - `deepseek-harness-web3-agent-stack`

Repo: [Haven-hvn/deepseek-harness-web3-agent-stack](https://github.com/Haven-hvn/deepseek-harness-web3-agent-stack)

Replaces `haven-core` and `haven-adapters`.

Sovereign Web3 agent harness — everything is a plug-in. Wallet custody (`dsh-wallet` + Ethereum OWS), treasury survival gradient, XMTP agent-per-conversation messaging, Synapse storage signing, Prowlarr/acquisition tools. Keys never leave the custody seam; config carries refs, per-operation signing only.

**Carry** - `haven-mobile`

Repo: [Haven-hvn/haven-mobile](https://github.com/Haven-hvn/haven-mobile)

Haven in your pocket. Native Android (Kotlin/Compose, `haven.mobile`) offline-first viewer — wallet connect, token-gated watch via haven-aol, Arkiv library/collections, Media3 playback, FOC-cache + Room, Keystore purged on disconnect. APKs ship via GitHub Releases + `android` workflow.

**Graduate** - `mint-glue-graduate`

Repo: [Haven-hvn/mint-glue-graduate](https://github.com/Haven-hvn/mint-glue-graduate)

pump.fun-style graduation for mint.club curves into locked Uniswap V4 liquidity via GlueHook — mint.club has no graduate, this is it. Launch token + pool + royalty-fed LP program in one tx (`RoyaltyRouterFactory.launch()`). Creator royalties auto-compound into permanently locked depth. Stale-token reclaim + DAO-capped fees by construction.

**Get involved**
The infrastructure is live. The pipes work — 5 clients, 4 networks, 0 private datastores.

Publish an archive with haven-cli, gate it with haven-aol, automate it on the harness, or launch a community drop with mint-glue-graduate — and show us what data portability looks like when the user actually owns the gate.

🌐 App: [haven.pinme.dev](https://haven.pinme.dev) · 📖 Docs: [haven-hvn.github.io/docs](https://haven-hvn.github.io/docs/) · 𝕏 [@havenplay3r](https://x.com/havenplay3r) · 📧 [officialhavennetwork@gmail.com](mailto:officialhavennetwork@gmail.com)
