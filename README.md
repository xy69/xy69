# Jaime Abril

Front end engineer based in Palma and Valencia, Spain, moving into AI agent deployment. TypeScript and Python.

I build agents that do real work, and I care about the unglamorous parts: tool design, validation, human approval, and what happens when the model fails. I have worked exclusively with coding agents for over a year, so I ship fast and verify carefully.

Now aiming at **forward deployed engineering**: taking agentic systems from pilot to production inside real organizations.

## Public work

| Project | What it is |
|---|---|
| [`tiny-agent`](https://github.com/xy69/tiny-agent) | Tiny, extensible AI agent in TypeScript. The core is the loop and the types; tools, loop detection, compaction and sub-agents are extensions. |
| [`tiny-agent-py`](https://github.com/xy69/tiny-agent-py) | The same idea in Python. Tools defined from pydantic models, async streaming, works with OpenRouter, Ollama and llama.cpp. Typed and tested. |

## Private work I'm happy to walk through

A notes, reminders and planning app driven by agents:

- Agents call the app's own API, so validation lives in one place
- The planner never writes: every change is a draft the user reviews and applies
- Skills (the open Agent Skills format) load on demand instead of bloating the prompt
- A failed 160-item import taught me to work in small batches with streamed progress and partial results

## Stack

TypeScript (browser, Node.js, Bun), Python, React, SQLite, OpenRouter, Ollama and llama.cpp on a local RTX 4090.

## Currently

Building an MCP-backed financial-crime alert triage agent with audit trail and approval UI, then evals for agent behavior.

Open to forward deployed engineering and agent deployment roles. [LinkedIn](https://www.linkedin.com/in/jaime-abril/)
