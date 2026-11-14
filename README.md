### Ilya Bondarenko — backend & AI engineer, Brno 🇨🇿

Backend systems and LLM features that run in production: queues, scrapers, model routing, retrieval, evals.
~5 years with TypeScript/Node.js (NestJS, BullMQ, PostgreSQL, Redis, AWS) and Kotlin/Spring; before that, dialogue systems and NLU at Just AI.

**How I build now:** AI agents (Claude Code, Codex) draft the specs, write the code and most of the tests. My part is deciding what gets built and what "done" means, steering the agents, reading the output, and catching what looks plausible but is wrong. Production calls and security stay with me.

#### Projects

| Project | What it is |
|---|---|
| [**JobScorer.app**](https://www.jobscorer.app) | Live product: scores job postings against a CV, drafts tailored CVs and screening answers. Langfuse tracing, evals, prompt-injection hardening. Code private; the guard rails are open below. |
| [**llm-job-fit-guards**](https://github.com/jawa7/llm-job-fit-guards) | The safety layer from JobScorer.app: SSRF-safe fetching of user URLs, typed validation of model output, prompt-injection evals, a rule that stops the model inventing years of experience. |
| [**shortform-qa**](https://github.com/jawa7/shortform-qa) | Deterministic QA for AI-made short videos: loudness (−14 LUFS), audio gaps, safe zones, unreadable text, voice-caption sync. Runs on a Czech news Shorts channel (~59k views). |
| [**harness**](https://github.com/jawa7/harness) | Agent loop for local models (stdlib Python): sandboxed tools, confirm-before-execute, eval suites with a judge model. Used to measure where small local models break. |
| [**crawler-with-api-and-mcp**](https://github.com/jawa7/crawler-with-api-and-mcp) | NestJS crawler + REST API + MCP server, so an agent can crawl and read pages through tools. |
| [**esp32-dht22-telemetry**](https://github.com/jawa7/esp32-dht22-telemetry) | Two ESP32 boards → ESP-NOW → Firebase → dashboard / Telegram Mini App. |

#### At work (private code)

- AI news pipeline: GPT-5 + vector dedup, cost-based routing across 4 models, multi-stage NestJS + BullMQ pipeline.
- Orchestrator for 15+ scraping processes (BullMQ, Puppeteer, retries, status tracking) across 5 social platforms.
- Real-time multiplayer duels with matchmaking and payments; XP/trophy engine with 40+ event types.

📫 [LinkedIn](https://linkedin.com/in/ilya-bondarenko-j7) · open to backend / AI engineering and solutions roles in Brno or remote (EU).
