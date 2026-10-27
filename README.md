# Stéphane Roche

Senior engineer, 11 years. **Wallets, Lightning and payments** is the spine of my work — from the first Bitcoin wallet extension at Ledger in 2015, to a Liquid wallet, a decentralised exchange protocol, agent payments, and a live product I run alone today.

Founder of Astral Horizon Labs.

---

## Selected work

**Ledger** · 2015, six-month internship
Contributed to Ledger's first Bitcoin wallet Chrome extension (CoffeeScript), with extensive unit testing.

**Bitcoin Studio** · 2017–2020 · Bitcoin & JavaScript consulting and training
Wrote the [BitcoinJS programming guide](https://github.com/bitcoin-studio/Bitcoin-Programming-with-BitcoinJS) used as professional course material. Built Lightning Network integrations, and wrote the Ansible playbooks that provision **LND and c-lightning** as reproducible machine images in [Bitcoin-VirtualMachine](https://github.com/bitcoin-studio/Bitcoin-VirtualMachine) (Packer, Vagrant Cloud, Hashicorp SSH keys).

**Marina — Liquid wallet** · 42 merged pull requests
Scaffolded the repository and its CI, built the full sending flow and the mnemonic handling, worked on UTXO balances with confidential-transaction unblinding, and **added Lightning support via Boltz submarine swaps**.
→ [my merged PRs](https://github.com/vulpemventures/marina/pulls?q=author%3Aastral-horizon-labs)

**TDEX — decentralised exchange protocol on Liquid** · 2020–2023
Merged PRs on the protocol's own **protobuf and swap-spec definitions**, on the Go daemon, and on the TypeScript SDK — where I compiled the daemon's spec into typed clients with Buf and protobuf-ts, built best-price discovery across liquidity providers, and replaced the coin selector. On the Liquid Development Kit: PSET fee and change computation, multisig address derivation, UTXO unblinding, and the peg-in scripts.
→ [my merged PRs](https://github.com/tdex-network/tdex-sdk/pulls?q=author%3Aastral-horizon-labs)

**BitGPT — agent payments** · 2025–2026
Main engineer on the dApp: an assistant that answers wallet and blockchain questions and then acts on them, with an agent layer I wrote — tools as typed modules with their own React renderers, an execution layer with follow-up and error handling, and the token allowance-and-approval flow that makes an agent's spending safe. Also built their **MCP desktop client** (Electron, MCP over stdio, wallets and contract calls), and 18 merged PRs on **h402**, their HTTP-402 payments standard (a fork of x402) — facilitator, express/hono/next middleware, fetch and axios interceptors, EVM presign transactions, Solana `signTransaction`.
→ [my merged PRs on h402](https://github.com/bit-gpt/h402/pulls?q=author%3Aastral-horizon-labs)

**Piko** · current, live
A multi-country marketplace I designed, built and operate alone: 180+ API endpoints, 200+ versioned SQL migrations, per-market payments and entitlements, six interface locales including Hebrew RTL. The backend enforces identity, ownership and quotas outside the prompt, so an assistant's tool calls can never exceed the user's real rights; model changes ship only behind per-market evaluations.
→ [pikosabe.com](https://pikosabe.com)

---

## How I work

- **Exactly once, or say so.** Retries are idempotent. A provider outcome that comes back ambiguous gets reconciled before anything is resent. Money movement is never assumed.
- **Read the spec, then find its gaps.** I would rather implement a young standard correctly than paper over it.
- **Own the whole path.** Interface, API, database, deployment — and I run it after it ships.

## Stack

TypeScript · Node · React · Vue/Nuxt · Kotlin Multiplatform · Compose · Tauri · Python · Go · Ruby
PostgreSQL / Supabase · Cloudflare Workers · Ansible · Packer · Docker
EVM · Solana · Bitcoin · Lightning · Liquid
LLM tool calling · LangChain · LlamaIndex · embeddings · evaluations

---

[astral-horizon-labs.com](https://astral-horizon-labs.com) · [LinkedIn](https://www.linkedin.com/in/stephane-roche/) · hello@astral-horizon-labs.com
