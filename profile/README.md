# HAVEN — Reclaiming the Internet for the user/agent.

Imagine your photos, videos, and notes live in a box you own, and you hold the only key. Right now most apps work the other way: you put your stuff in *their* box, they keep the key, and if they close or get greedy, you're stuck.

We build free, open tools that flip that back. Your stuff is locked before it ever leaves your computer. Nobody — not us, not a big company — can open it without the key. And the key is you or your AI Agent.

Docs: https://haven-hvn.github.io/docs/

### 📈 Trending

[![vlm-engine PyPI Downloads](https://img.shields.io/badge/downloads-2k_/month-blue)](https://pypistats.org/packages/vlm-engine)

*[vlm-engine](https://github.com/Haven-hvn/haven-vlm-engine-package)* is gaining traction — over 2,000 downloads per month on PyPI.

### 🚀 The Tools
**Read** — haven-dapp

Repo: [Haven-hvn/haven-dapp](https://github.com/Haven-hvn/haven-dapp)

Site: [https://haven.pinme.dev](https://haven.pinme.dev)

Your videos, decentralized. No sign-up, no password — your wallet is your name and your key. Anyone can watch the free shelf; locked videos open only if you hold the right thing. The player is just a window; your library lives somewhere else, so a different window can open the same library tomorrow. Includes a Publish a Drip wizard + Upcoming Video Drops: each release splits into 1–10 chunks that stay locked until its mint.club market cap hits that chunk's goal, then that chunk's key unlocks. The whole site is pinned to IPFS, caches for offline use, unlocks in batches.

**Write** — haven-cli

Repo: [Haven-hvn/haven-cli](https://github.com/Haven-hvn/haven-cli)

The only part that does the locking. Archiving and automation that runs on your own machine — no server somewhere that can kick you out. It looks at a file, tags it, locks it, uploads it, and keeps your list in sync. Local SQLite, scheduled runs, plug-ins.

**Own** — haven-aol

Repo: [Haven-hvn/haven-aol](https://github.com/Haven-hvn/haven-aol)

Canister smart contract: [gny6k-fqaaa-aaaab-ag3ra-cai](https://dashboard.internetcomputer.org/canister/gny6k-fqaaa-aaaab-ag3ra-cai)

The lock itself. Real ownership needs privacy — otherwise your stuff is just public. This little program checks your wallet, sees what you hold, and only then hands over the key. You decide who gets in, and the lock keeps working even if the website is gone.

- v1: one key per file
- v3: one key opens a whole collection for 30 days, remembered after that
- v4: keys unlock chunk by chunk as the market cap climbs; if the price check fails, the door stays shut
- Portable Ed25519 proofs so you can show you hold something without asking for the key again

**Synthesize** — haven-vlm-engine

Repo: [haven-vlm-engine-package](https://github.com/Haven-hvn/haven-vlm-engine-package)

A robot helper that looks at your files for you — tags, details, sorting — without sending anything to a company. Runs on a normal computer, no fancy hardware, spreads work out and keeps going if one helper fails. Powers haven-cli analyze.

**Automate** — deepseek-harness-web3-agent-stack

Repo: [Haven-hvn/deepseek-harness-web3-agent-stack](https://github.com/Haven-hvn/deepseek-harness-web3-agent-stack)

A helper robot that does chores for you — wallet, storage, messaging, finding files — and everything is a plug-in you can swap. The keys never leave one safe spot; the robot asks for one small signature at a time instead of holding everything.

**Carry** — haven-mobile

Repo: [Haven-hvn/haven-mobile](https://github.com/Haven-hvn/haven-mobile)

Haven in your pocket. An Android app that works offline — connect your wallet, watch what you're allowed to watch, keep a library. Same wallet, same stuff, same permissions as everywhere else. The key is wiped from the phone the moment you disconnect. APKs ship via GitHub Releases.

**Earn** — mint-glue-graduate

Repo: [Haven-hvn/mint-glue-graduate](https://github.com/Haven-hvn/mint-glue-graduate)

pump.fun-style graduation for mint.club curves into locked Uniswap V4 liquidity via GlueHook — mint.club has no graduate, this is it. Launch token + pool + royalty-fed LP program in one tx (RoyaltyRouterFactory.launch()). Creator royalties auto-compound into permanently locked depth. Stale-token reclaim + DAO-capped fees by construction.

🧪 The one question that matters

Forget whether something uses a blockchain. Ask this instead:

**If the company vanishes tomorrow, or gets mean, can someone else still show you your stuff?**

That takes real work: files you can actually reach, labels you can actually read, locks anyone can rebuild, and more than one app worth using.

Some things still can't be fixed. Once someone has seen a file, taking the key back doesn't unsee it. And holding a token isn't the same as owning the copyright.

Get involved The pipes already work — 5 apps, 4 networks, 0 private servers holding your stuff.

Publish an archive with haven-cli, lock it with haven-aol, automate it with the robot, or start a community drop with mint-glue-graduate — and show us what it looks like when you own the key.

**Apps should be guests in your world. Not you in theirs.**


🌐 App: [haven.pinme.dev](https://haven.pinme.dev) · 📖 Docs: [haven-hvn.github.io/docs](https://haven-hvn.github.io/docs/) · 𝕏 [@havenplay3r](https://x.com/havenplay3r) · 📧 [officialhavennetwork@gmail.com](mailto:officialhavennetwork@gmail.com)
