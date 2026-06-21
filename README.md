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
