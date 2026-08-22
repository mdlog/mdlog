# mdlog

**Web3 security · payment rails for autonomous agents**

I audit smart contracts and build the infrastructure that lets AI agents pay for what
they use. Most of my work sits where those two meet: agent-to-agent payments over
HTTP 402 (x402), on-chain identity and reputation (ERC-8004), and the guardrails that
stop an autonomous system from doing something expensive and irreversible.

39 repositories saw work in 2026, across Casper, 0G, Starknet, Midnight, BNB Chain and
X Layer.

---

## Shipped

| Project | What it does | Stack | Status |
| :-- | :-- | :-- | :-- |
| **[AgentGate](https://github.com/mdlog/AgentGate)** | Turns any HTTP API into a paid on-chain service in one command — HTTP 402 micropayments in CSPR, with a service registry and payment-backed reputation | Casper · Odra · TypeScript | [Live demo](https://agentgate.mdloglabs.org) · [`@mdlog/agentgate`](https://www.npmjs.com/package/@mdlog/agentgate) · Casper testnet |
| **[AgentDock](https://github.com/mdlog/agentdock)** | Marketplace for ERC-8004 agents — find one that does a specific job, see evidence it works, hire it from your own wallet. No custody and no token approvals: every payment is an EIP-3009 authorization you sign in your browser | BNB Smart Chain · Python | [Live](https://agents.mdloglabs.org) |
| **[ExitGuard](https://github.com/mdlog/ExitGuard)** | The seatbelt a trading agent calls before it becomes exit liquidity — answers whether it can actually *exit* at that size, returning BLOCK / WARN / OK plus an auditable depth curve, billed per call | X Layer · x402 · USDT0 · MCP | OKX.AI Agentic Service Provider |
| **[ShadowAgents](https://github.com/mdlog/ShadowAgents)** | Private payroll — pay a whole team in one transaction without publishing the org chart: who is on it, what each person earns, or when they were paid | Starknet · STRK20 privacy pool | Mainnet |
| **[aegis-vault](https://github.com/mdlog/aegis-vault)** | Verifiable-AI risk manager with autonomous execution guardrails | 0G Aristotle mainnet · Solidity | [Contract](https://chainscan.0g.ai/address/0x9e36520650Fd7d06CA77Fb0045456c03d3582A5F) |
| **[eip7702-rescue](https://github.com/mdlog/eip7702-rescue)** | Claims and evacuates assets from a wallet running an attacker's EIP-7702 sweeper — atomically, in one transaction, without ever funding the compromised address | Solidity · Foundry | Recovery tool |
| **[alibi](https://github.com/mdlog/alibi)** | Proves an agent refused an order without revealing the order, the policy, or where the policy lives | Midnight · Compact · ZK | In progress |

---

## Security work

Smart contract auditing and bug bounty hunting, mostly DeFi.

- **What I hunt** — accounting desync, invariants broken across coupled state, incomplete
  code paths, oracle and flash-loan assumptions, signature replay, proxy and upgrade footguns
- **How I report** — proof of concept first. If I cannot write a Foundry test that fails
  against the vulnerable contract and passes against the patched one, it does not get submitted
- **Where it shows up in my own code** — `eip7702-rescue` and `ExitGuard` both exist because
  the attack came first and the tool came second

---

## Stack

| | |
| :-- | :-- |
| **Contracts** | Solidity · Rust · Cairo · Compact · Odra |
| **Application** | TypeScript · Next.js · Node · Python |
| **Security** | Foundry · Slither · Hardhat |
| **Chains** | Ethereum · BNB Chain · Starknet · Casper · 0G · Midnight · X Layer |

---

## Stats

<p>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=mdlog&theme=github_dark" />
    <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=mdlog&theme=default" alt="GitHub profile summary for mdlog" width="700" />
  </picture>
</p>

<p>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=mdlog&theme=github_dark" />
    <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=mdlog&theme=default" alt="Repositories per language" width="340" />
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=mdlog&theme=github_dark" />
    <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=mdlog&theme=default" alt="Most used languages by commit" width="340" />
  </picture>
</p>

---

## Contact

Audit enquiries, agent-infrastructure work, or questions about anything above:

**[dev@mdloglabs.org](mailto:dev@mdloglabs.org)**
