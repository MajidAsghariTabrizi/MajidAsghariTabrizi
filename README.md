# Majid Asghari Tabrizi

```text
$ whoami
builder > systems engineer > DeFi architect

$ focus
autonomous trading > MEV infrastructure > smart contracts > production observability
              > AI infrastructure > LLM tooling

$ status
shipping open-source AI infrastructure > building on-chain systems that operate without human intervention
```

<div align="center">

[![GitHub followers](https://img.shields.io/github/followers/MajidAsghariTabrizi?style=for-the-badge&logo=github&color=1f6feb)](https://github.com/MajidAsghariTabrizi)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/majid-asghari)

</div>

---

## What I Build

**Autonomous On-Chain Systems** -- Production-grade agents that detect, validate, and execute DeFi opportunities in real-time. Every submission is mathematically verified through fork simulation and dual-provider agreement before it touches the chain.

**MEV & Liquidation Intelligence** -- Independent revenue lanes for Aave V3 liquidations, Atlas auction solving, and origin-aware V3 arbitrage. Each lane has its own armed state, kill switch, economic gate, and operational controls.

**Smart Contract Infrastructure** -- Solidity executors with minimum-profit guards, on-chain automation, and Foundry-based development with comprehensive fork test coverage.

**Distributed Systems & Observability** -- Multi-service architectures with NATS event streaming, PostgreSQL as economic truth, Prometheus metrics, and real-time dashboards. Systems that never sleep, and never lie about what they are doing.

**AI Infrastructure & LLM Tooling** -- Open-source routers, agents, and production integrations that turn the messy reality of LLM providers into a stable, observable product surface. Built for developers who want free AI capabilities without the operational complexity.

---

## Featured Work

<table>
<tr>
<td width="50%" valign="top">

### [universal-engineering-agent](https://github.com/MajidAsghariTabrizi/universal-engineering-agent)
**Open-source engineering-agent operating kernel**

A standalone, MIT-licensed reference implementation of the 9-stage UEA operating-kernel contract. Profile-agnostic, runnable, zero runtime dependencies.

- 9 stages: inspect, plan, implement, tool-hygiene, verify, classify, recover, test, generalize
- 10-class deterministic failure classifier (no model inference, no network call)
- Bounded recovery with non-retryable fall-through
- Staged verification reading commands from your own package.json
- 31 self-tests under plain node --test
- 6-command CLI: inspect, plan, verify, classify, test, scan
- 3 example missions + 1 sample workspace + 1 reference profile
- Sibling to free-best-router (model routing vs. engineering coordination)

`Node.js` `Operating Kernel` `Verification` `Failure Classification` `Profile-Driven` `DeepSeek Harness`

**v0.1.0 released** -- MIT -- Public

</td>
<td width="50%" valign="top">

### [free-best-router](https://github.com/MajidAsghariTabrizi/free-best-router)
**Open-source intelligent router for free AI models**

One OpenAI-compatible endpoint that automatically discovers, ranks, health-checks, and routes to the best available free model across OpenRouter, OpenCode/Zen, Groq, Cerebras, Mistral, DeepSeek, and local inference servers.

- 7-component capability-aware scoring (capability x reliability x latency)
- Wilson lower bound on success rate + Bayesian shrinkage for under-sampled candidates
- Per-failure-type cooldowns (429 = 8 min, 404 = 1 h) with exponential backoff
- Smart exploration -- 5% of requests probe non-incumbent healthy candidates
- Bounded failover -- 4 attempts x 45 s = 180 s wall time per request
- 52 unit tests -- GitHub Actions CI -- 17 SEO topics
- DeepSeek Harness first-class integration

`Node.js` `OpenAI-compatible` `LLM Gateway` `Multi-Provider` `Smart Routing`

**v0.1.0 released** -- MIT -- Public

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [anti-gravity-phoenix-v4](https://github.com/MajidAsghariTabrizi/anti-gravity-phoenix-v4)
**Autonomous MEV agent on Arbitrum**

Fork-simulates liquidation routes, evaluates economics with conservative PnL gates, and executes with fail-closed controls. Three independent revenue lanes:
- `aave_liquidation` -- Aave V3 liquidation intelligence
- `atlas_solver` -- Atlas auction monitoring and solving
- `phoenix_dex` -- V3-style origin-aware arbitrage research

`Rust` `Solidity` `Go` `Python` `PostgreSQL` `NATS` `Docker`

2 stars -- 14 open issues -- Active

</td>
<td width="50%" valign="top">

### [smart-trader](https://github.com/MajidAsghariTabrizi/smart-trader)
**Algorithmic trading system**

Market analysis and automated decision-making for on-chain opportunities. Built around deterministic evaluation and bounded risk.

`Python` `Trading Logic` `Market Data` `Risk Controls`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [GMX](https://github.com/MajidAsghariTabrizi/GMX)
**Perpetual DeFi integration**

Direct integration with GMX -- one of the largest on-chain perpetual exchanges. Real infrastructure that interacts with real liquidity.

`Python` `DeFi` `Perpetuals` `On-chain Execution`

</td>
<td width="50%" valign="top">

### [Arbitrum](https://github.com/MajidAsghariTabrizi/Arbitrum)
**Where it started**

Product management and web development work on the Arbitrum ecosystem. The L2 where everything else runs. Foundation for 5+ years of on-chain building.

`Product` `Web Dev` `L2` `Ecosystem`

</td>
</tr>
</table>

---

## The UEA + Free Best Router Ecosystem

```
DSH session
  +-- UEA kernel (engineering loop)
        +-- llm block --> free-best-router --> upstream free providers
```

| Project | Answers |
|---|---|
| [universal-engineering-agent](https://github.com/MajidAsghariTabrizi/universal-engineering-agent) | How should the agent perform engineering work reliably? |
| [free-best-router](https://github.com/MajidAsghariTabrizi/free-best-router) | Which model should the agent use? |

They are siblings. Stack, not overlap.

---

## Technical Stack

**Languages**
`Rust` `Python` `TypeScript` `Solidity` `Go` `JavaScript`

**Backend & Infrastructure**
`FastAPI` `Node.js` `PostgreSQL` `Docker` `GitHub Actions` `Linux` `NATS JetStream`

**AI / LLM Infrastructure**
`Node.js` `OpenAI-Compatible APIs` `Multi-Provider Routing` `LLM Gateway Design` `Capability-Aware Ranking` `Runtime Health Models` `Streaming & Tool-Calling` `DeepSeek Harness`

**Blockchain & DeFi**
`Arbitrum` `Aave V3` `Foundry` `Ethers.js` `Uniswap V3` `GMX` `Atlas`

**Data & Observability**
`Metabase` `Kibana` `Prometheus` `Real-time Dashboards` `Event Processing`

**AI & Automation**
`LLM Integration` `Autonomous Agents` `Event-driven Systems`

---

## Engineering Principles

```text
Build systems that are observable.
Automate what should not require humans.
Prefer simple architectures over unnecessary complexity.
Measure outcomes, not activity.
Ship > observe > learn > improve.
```

**Safety invariants I refuse to compromise on:**
- Two independent providers required for any authority-bearing decision
- Provider disagreement closes execution authority until fresh agreement
- One global submission lock prevents conflicting transactions
- Realized PnL recorded only after receipt and balance reconciliation
- Unknown state blocks new authority -- no-alpha is not an error

---

## AI-Assisted Engineering

I am an AI-assisted engineer. AI accelerates implementation, testing, debugging, and documentation. But **product definition, architecture, economic policy, risk boundaries, and operational decisions remain human-owned**.

The question I keep exploring: *How can a product-oriented builder coordinate financial engineering, blockchain infrastructure, and distributed systems with a much smaller team surface?*

Phoenix is the answer I am shipping.
free-best-router and universal-engineering-agent are the next ones.

---

## GitHub Activity

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=MajidAsghariTabrizi&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=58a6ff&icon_color=79c0ff&text_color=c9d1d9&ring_color=1f6feb&include_all_commits=true&count_private=true"/>
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MajidAsghariTabrizi&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&langs_count=8"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com/?user=MajidAsghariTabrizi&theme=tokyonight&hide_border=true&background=0d1117&ring=58a6ff&fire=ff6b35&currStreakLabel=58a6ff)](https://git.io/streak-stats)

</div>

---

## Current Focus

```text
Phoenix v4           > continuous protected LIVE hunting
Aave lane            > armed, economic gate enforced
Atlas solver         > armed, auction stream connected
free-best-router     > v0.1.0 shipped, community adoption phase
universal-engineering-agent > v0.1.0 shipped, DSH ecosystem launch
LLM tooling          > next-gen agent infrastructure
```

**The terminal state I am working toward:**
```text
FIRST_POSITIVE_REALIZED_PNL
```
Valid only after: real transaction submitted > confirmed > balance-reconciled > positive net PnL recorded.

A healthy production system can legitimately remain in:
```text
FULLY_LIVE_NO_ALPHA
```
Live. Authority available. No opportunity currently passing every gate. **That is correct behavior.**

---

## Connect

- [LinkedIn](https://www.linkedin.com/in/majid-asghari) -- for professional conversations
- [GitHub](https://github.com/MajidAsghariTabrizi) -- for code and technical discussion
- Open to interesting DeFi infrastructure, autonomous systems, and AI-assisted engineering conversations

---

<div align="center">

**Built with curiosity. Shipped with care.**

```text
$ uptime
5+ years in the chain
$ _
```

</div>
