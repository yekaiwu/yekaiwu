<div align="center">

# Wu Yekai

**Software engineer building agentic products, decision systems, and data-rich tools.**

[Portfolio](https://yekaiwu.github.io) · [GitHub](https://github.com/yekaiwu) · [LinkedIn](https://www.linkedin.com/in/yekaiwu/) · [Email](mailto:wuyekai.sg@gmail.com) · [Résumé](https://yekaiwu.github.io/uploads/resume.pdf)

</div>

I take systems from problem framing through architecture, implementation, testing, and usable interfaces. Recent work includes a workflow-configured real-estate engagement agent, a calibration-first forecasting engine, a multimodal transit router, and full-stack LLM applications.

## Technical focus

- **Agentic and LLM systems:** versioned workflows, structured tool use, prompt/runtime boundaries, deterministic fallbacks, and evaluation gates.
- **Decision and quantitative systems:** calibration, probability forecasting, market-data pipelines, risk controls, backtesting, and explainable recommendations.
- **Backend and data:** Python, TypeScript, FastAPI, Next.js, Node.js, PostgreSQL, SQLite, Supabase, API integrations, and typed contracts.
- **Product engineering:** React, Vite, responsive interfaces, operational dashboards, browser automation, CI, and reproducible local setup.

## Featured work

| Project | Problem and solution | Engineering evidence |
| --- | --- | --- |
| [Realtor OS](https://yekaiwu.github.io/#realtor-os) | Gives property agents one desk for inbound WhatsApp/voice leads, AI-led qualification, bookings, follow-ups, inventory, and CRM sync. | Config-to-runtime workflow compiler; per-thread version pinning; Vercel AI SDK/OpenRouter tool loop; Twilio, Cal.com, and Twenty adapter boundaries; local deterministic runtime; typecheck, Vitest, and E2E scripts. |
| [Jump Cup](https://yekaiwu.github.io/#case-jump) | Turns natural-language football markets into calibrated probabilities rather than winner picks. | LLM + heuristic parser path, model routing, confidence-weighted ensemble, isotonic calibration, shrinkage, and an inspectable trace. Its calibration gate evaluates 198 settled markets across 20 matches and rejects non-finite forecasts or defined Brier-score regressions. |
| [Money Money](https://yekaiwu.github.io/#case-money) | Personal, multi-market research and portfolio decision support for a SGD-based retail account. | Pluggable strategies, point-in-time price access, aggregation and risk gates, monitoring, backtest/effectiveness modules, FastAPI + Jinja/HTMX dashboard, and an optional LLM explainer constrained to structured facts. |
| [Chess Coach](https://github.com/yekaiwu/Chess_Coach) | Makes engine analysis usable as coaching by pairing chess evaluation with context-aware explanation. | React/TypeScript + FastAPI system; Stockfish analysis orchestrated with provider-configurable LLM chains; structured outputs, conversation memory, Docker configuration, and backend/frontend/integration CI workflows. |

## Other projects

| Project | What it demonstrates |
| --- | --- |
| [MRT + Bus Router](https://yekaiwu.github.io/#case-mrt) | Singapore leave-now routing across live LTA bus arrivals, GTFS rail schedules, OneMap walking, and a checkpointed Google Maps benchmark. It explicitly documents data-quality limits. |
| WC26 Edge | Market-first betting decision support: de-vigged sharp-book consensus, Dixon-Coles pricing, append-only odds snapshots, CLV tracking, and capped quarter-Kelly recommendations. Research tool only—not financial advice. |
| [Job Application Assistant](https://yekaiwu.github.io/#job-app) | In-progress FastAPI/SQLite/React job-search workflow with public-ATS connectors, factual Qwen-assisted bullet tailoring, PDF rendering, and a KNOWN / INFERABLE / PERSONAL-UNKNOWN form-field router. |
| Bojio / Food Buddy | Mobile-first social dining product with Supabase phone OTP, row-level security, restaurant parsing, host approval, and real-time meal chat. |
| NUS Tennis Booker | Time-critical Playwright automation with persistent sessions, a pre-warmed browser pool, scheduled court search, health checks, payment handoff, and Telegram alerts. |
| [Claude When](https://github.com/yekaiwu/claude_when) | A local-first TypeScript/Express scheduler that starts a Claude Code CLI session on a daily cron and surfaces schedule state through a small web UI. |
| Liquidity | An architecture-first autonomous trading-agent track with a deterministic risk ladder, typed execution boundary, safety invariants, and specification-led tests. |

## Engineering quality signals

- Project repositories contain tests, typed interfaces, setup instructions, and documented system boundaries—not just demos.
- `Jump Cup` treats calibration as a merge gate; `MRT + Bus Router` preserves benchmark checkpoints and caveats; `Realtor OS` has automated typecheck/test workflows and scenario scripts.
- `Chess Coach` includes CI for backend, frontend, integration, and dependency-security checks. This portfolio is built and deployed through GitHub Pages workflows.

## GitHub activity

- [Public profile and contribution history](https://github.com/yekaiwu)
- [Portfolio source](https://github.com/yekaiwu/yekaiwu.github.io) and [Chess Coach](https://github.com/yekaiwu/Chess_Coach) are linked only because their public URLs are verifiable. Other case studies remain documented here and on the portfolio while their source links are not publicly accessible.

## Current interests

Reliable agentic systems, especially workflow versioning, tool safety, observable decision paths, and evaluation. I’m equally interested in the quantitative side of decision-making: calibration, backtesting, risk constraints, and honest measurement.

## Contact

For software engineering, AI engineering, data, quantitative, or product-focused technical roles:

- [Portfolio](https://yekaiwu.github.io)
- [GitHub](https://github.com/yekaiwu)
- [LinkedIn](https://www.linkedin.com/in/yekaiwu/)
- [wuyekai.sg@gmail.com](mailto:wuyekai.sg@gmail.com)
