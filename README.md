<div align="center">

# Hi, I'm Roland 👋

### I build open-source tooling for LLM agents.

Small, sharp, local-first tools for people who ship agents and need to see
what they're actually doing.

</div>

---

### 🧰 The LLM-agent toolkit

Sharp, local-first tools — lint your tools, capture a run, replay it, and fix what's slow.

| | what it does |
|---|---|
| 🧹 **[toollint](https://github.com/oavlloh-wq/toollint)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/toollint?style=flat&label=★) | Linter for tool / function-calling schemas — catches the mistakes that make agent tool-calls **silently fail**. Anthropic + OpenAI dialects, zero deps. |
| 🚰 **[llmtap](https://github.com/oavlloh-wq/llmtap)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/llmtap?style=flat&label=★) | Transparent proxy — record every Anthropic API call with **zero code change** (one env var). Streaming-aware, live cost/cache dashboard. |
| ⏪ **[rewind](https://github.com/oavlloh-wq/rewind)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/rewind?style=flat&label=★) | Time-travel debugger — inspect any step of a recorded run, then **fork & replay** it with edits to ask "what if?" |
| 🔍 **[cachelens](https://github.com/oavlloh-wq/cachelens)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/cachelens?style=flat&label=★) | Prompt-cache doctor — finds **why your cache isn't hitting** and how much it's costing you. |
| 💧 **[trickle](https://github.com/oavlloh-wq/trickle)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/trickle?style=flat&label=★) | Best-effort parser for **partial / streaming JSON** — read tool-call fields *as they stream in*, before the closing brace. Zero deps. |
| ✂️ **[ctxfit](https://github.com/oavlloh-wq/ctxfit)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/ctxfit?style=flat&label=★) | Trim conversation history to a token budget **without breaking it** — never orphans a `tool_use`/`tool_result` pair. Zero deps. |
| ✅ **[msglint](https://github.com/oavlloh-wq/msglint)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/msglint?style=flat&label=★) | Pre-flight validator for the Anthropic Messages API — catches the **structural bugs that cause 400s** (bad alternation, dangling `tool_use`, system-in-messages) before you send. Zero deps. |
| 🕶️ **[cloak](https://github.com/oavlloh-wq/cloak)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/cloak?style=flat&label=★) | **Reversibly redact secrets & PII** from prompts before they leave your machine — keys, emails, cards, IPs → stable placeholders, restored when the model echoes them back. Zero deps, offline. |
| 🌀 **[spincheck](https://github.com/oavlloh-wq/spincheck)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/spincheck?style=flat&label=★) | Catch an agent **stuck in a loop** — repeats, `A-B-A-B` cycles, low-novelty churn — before it burns your token budget. Watches the tool-call stream, trips with a reason. Zero deps. |
| 🔧 **[coax](https://github.com/oavlloh-wq/coax)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/coax?style=flat&label=★) | **Repair & coerce tool-call arguments** to match your JSON Schema — `"5"`→`5`, `"yes"`→`true`, stringified-JSON→object, scalar→array, wrong-case enums. Fixes the type wobble that throws in your handler, with an audit trail. Zero deps. |
| 🥫 **[canned](https://github.com/oavlloh-wq/canned)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/canned?style=flat&label=★) | **Deterministic, offline test double for the Anthropic Messages API** — script replies (tool calls included), drop the stub in where your code wants a client, assert on what the agent did. No API key, no network. Zero deps. |
| 📼 **[streamfold](https://github.com/oavlloh-wq/streamfold)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/streamfold?style=flat&label=★) | **Reconstruct the final Anthropic message from a recorded SSE stream** — folds `text`/`tool_use`/`thinking` deltas + usage back into one message, and flags truncated or corrupt streams. Offline, zero deps. |
| 🧾 **[tariff](https://github.com/oavlloh-wq/tariff)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/tariff?style=flat&label=★) | **Cost calculator for Anthropic API usage logs** — turns logged `usage` into dollars with the **cache tiers done right** (read 0.1×, write 1.25×/2×, batch 0.5×). Digs records out of messy logs, groups by model. No key, offline, zero deps. |
| 🧬 **[schemize](https://github.com/oavlloh-wq/schemize)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/schemize?style=flat&label=★) | **Infer a JSON Schema from example JSON values** — feed it a sample tool output or API response and get a clean draft-2020-12 schema for your **tool params / structured outputs**. Merges examples (required vs optional, null/number unions), detects formats. Offline, zero deps. |
| 🔁 **[transmute](https://github.com/oavlloh-wq/transmute)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/transmute?style=flat&label=★) | **Convert chat payloads between OpenAI and Anthropic** — moves the system prompt, rewrites `tool_calls`↔`tool_use`, `role:"tool"`↔`tool_result`, images and tool defs, and fixes role alternation so the other provider just accepts it. Both directions, offline, zero deps. |
| 🔬 **[promptdiff](https://github.com/oavlloh-wq/promptdiff)** &nbsp;![stars](https://img.shields.io/github/stars/oavlloh-wq/promptdiff?style=flat&label=★) | **Structure-aware diff of two Anthropic Messages API requests** — skips the JSON-formatting noise and shows what actually changed: model/params, tools added/removed/retyped, a word-level system-prompt diff, and message inserts/edits. Offline, zero deps. |

```
llmtap (capture)  →  rewind (replay)  →  cachelens (optimize)
```

---

### 🛠 Working with

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-d97757?logo=anthropic&logoColor=white)
![LLM Agents](https://img.shields.io/badge/LLM_Agents-111?logo=robotframework&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)

---

<div align="center">

![stats](https://github-readme-stats.vercel.app/api?username=oavlloh-wq&show_icons=true&hide_border=true&theme=transparent&count_private=true)
![langs](https://github-readme-stats.vercel.app/api/top-langs/?username=oavlloh-wq&layout=compact&hide_border=true&theme=transparent)

</div>
