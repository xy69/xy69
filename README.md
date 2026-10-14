# Jaime Abril

Palma, Spain · Front end engineer building production AI agents · TypeScript, Python

I build agents that do real work, and I care most about the unglamorous part: tool design, validation, human approval, graceful failure, and making sure the thing is still useful at 2 a.m. when a model misbehaves.

I have worked exclusively with coding agents for over a year (writing, testing, verifying, and reviewing end to end), so I ship quickly and keep a tight check on quality.

Right now I'm moving into **forward deployed engineering**: taking agentic systems from pilot to production inside real organizations.

## What I work on

- **Agent engineering:** tool calling, structured output, streaming, multi-step loops, context management, skill catalogues
- **Human-in-the-loop design:** agents that propose, people approve; drafts instead of direct writes; confirmation before anything destructive
- **Models, hosted and local:** OpenRouter in daily use; Ollama and llama.cpp on a local RTX 4090
- **Full-stack TypeScript:** browser, Node.js and Bun; React; SQLite; PWAs with push notifications and a private gateway

## Public work

| Project | What it is |
|---|---|
| [`tiny-agent`](https://github.com/xy69/tiny-agent) | A tiny, extensible AI agent in TypeScript. The core is only the loop and the types; everything else is an extension (tools, loop detection, compaction, sub-agent delegation). Works with any OpenAI-compatible API or Anthropic. MIT. |

More coming: a Python port, evals tooling, and write-ups of what I learn deploying agents.

## Private work (available to discuss)

Most of what I build lives in private repos. The one I'm happiest to walk through is a notes, reminders and planning app driven by agents:

- Agents with 8 to 17 tools reach the domain through the app's own API, so validation lives in one place, and stream over SSE
- A planning agent that **never writes**: every change comes back as a validated draft the user reviews, edits and applies
- A skills catalogue following the open Agent Skills format, loaded on demand instead of stuffing the system prompt
- Reminders that fire through an agent and fall back to a plain notification if the model or its key is unavailable
- A documented redesign after a real failure: a model truncated its JSON halfway through a long import, so the work moved to small batches with streamed progress and partial results

## Lessons I keep relearning

- Asking a model for the whole answer in one response is a design bug, not a prompt bug.
- A draft the user can reject is worth more than an autonomous write.
- Fallbacks need the same care as the happy path.
- If you cannot measure it, you do not know that it works.

## Currently

- Building evals for agent behavior
- Deploying agents on cloud infrastructure with proper security review
- Writing down what breaks

Open to conversations about forward deployed engineering and agent deployment roles. Find me on [LinkedIn](https://www.linkedin.com/in/jaime-abril/).
