<div align="center">

# Wu Yekai

**Software engineer building agentic products, decision systems, and data-rich tools.**

[Portfolio](https://yekaiwu.github.io) &nbsp;·&nbsp; [LinkedIn](https://www.linkedin.com/in/yekaiwu/) &nbsp;·&nbsp; [Email](mailto:wuyekai.sg@gmail.com)

</div>

<br>

## Selected projects

<table>
<tr>
<td width="50%" valign="top">

<img src="assets/realtor-os-workflows.png" width="100%" alt="Realtor OS workflow library showing versioned seller qualification, buyer qualification, and listing enquiry workflows">
<sub>Workflow configuration screen: versioned prompts, stages, and tools.</sub>

### Realtor OS

A lead-engagement operating desk for property agents — inbound WhatsApp and voice leads, assistant-led qualification, bookings, inventory, cost visibility, and CRM sync in one runtime.

- Workflow compiler renders a versioned prompt, workflow definition, and runtime variables into a system prompt and tool set; each conversation pins its own version so a live thread never shifts mid-conversation.
- Runs fully offline on a local JSON store and deterministic mock providers, covered by Vitest units plus smoke, readiness, and route-level E2E suites.

<code>Next.js</code> <code>Vercel AI SDK</code> <code>Twilio</code> <code>Postgres</code> <code>Twenty CRM</code>

</td>
<td width="50%" valign="top">

<img src="assets/jump-cup-brier.png" width="100%" alt="Jump Cup evaluation chart comparing mean crowd Brier score across settled-market question families">
<sub>Calibration gate output: crowd forecasting error by question family.</sub>

### Jump Cup

A multi-model probability-forecasting engine for World Cup markets, built around Brier-score calibration rather than confident winner picks.

- Question parser (LLM + heuristic, cross-checked) routes into 8 model families, ensembles their outputs, then applies isotonic calibration and base-rate shrinkage.
- A calibration gate fails the build unless engine Brier score beats crowd consensus across 198 settled markets from 20 captured matches.

<code>Python</code> <code>scikit-learn</code> <code>OpenRouter</code> <code>SQLite</code>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<img src="assets/chess-coach.png" width="100%" alt="Chess Coach interface showing the game board and position evaluation panel">
<sub>Evaluation tab: live win-probability and centipawn scoring.</sub>

### [Chess Coach ↗](https://github.com/yekaiwu/Chess_Coach)

A full-stack chess coach that turns Stockfish evaluations into contextual commentary, tactics, and a coaching chatbot.

- FastAPI backend coordinates Stockfish analysis with LangChain-based chat, exposing evaluation, commentary, tactics, and chat as separate routes consumed by a React/TypeScript client.
- Dockerized local setup with separate backend, frontend, and integration CI workflows, plus a scheduled security scan.

<code>React</code> <code>TypeScript</code> <code>FastAPI</code> <code>Stockfish</code> <code>LangChain</code>

</td>
<td width="50%" valign="top">

<img src="assets/mrt-bus-router.png" width="100%" alt="MRT and Bus Router diagram showing a multi-modal route from origin to destination with bus, MRT, and walking legs, plus a 42-win/29-tie/29-loss benchmark against Google Maps">
<sub>Route search and benchmark vs. the Google Maps Routes API.</sub>

### [MRT + Bus Router ↗](https://github.com/yekaiwu/mrt-bus)

"Leave now" Singapore transit routing over a custom bounded multi-modal search — live LTA bus arrivals, GTFS rail topology, and OneMap walking data — with zero third-party runtime dependencies.

- Priority-queue label search with transfer penalties and same-mode vs. cross-mode walking caps, bounded to 1,500 search labels to keep live LTA quota usage predictable.
- Benchmarked against the Google Maps Routes API on 100 checkpointed cases: 42 wins · 29 ties · 29 losses, avg +1.1 min.

<code>Python (stdlib)</code>

</td>
</tr>
</table>

<table>
<tr>
<td width="42%" valign="top">

<img src="assets/nus-tennis-booker.png" width="100%" alt="NUS Tennis Booker timeline diagram showing pre-warm, window open, slot polling, and Telegram handoff steps">
<sub>Race timeline: pre-warm through Telegram handoff.</sub>

</td>
<td width="58%" valign="top">

### [NUS Tennis Booker ↗](https://github.com/yekaiwu/nus_tennis)

Playwright automation that races a university tennis-court booking portal the instant slots release, then hands the payment step to a human over Telegram.

- Pre-warms and parks an authenticated session ahead of the release window, then polls the slot grid every 200ms once it opens — saving the launch and navigation time that would otherwise cost the race.
- A separate scheduled health-check job re-authenticates and asserts the slot grid's DOM hasn't changed, alerting over Telegram if the site breaks.

<code>Python</code> <code>Playwright</code> <code>APScheduler</code> <code>FastAPI</code>

</td>
</tr>
</table>

<sub>Also maintain a small local scheduler that triggers daily Claude Code CLI sessions via <code>node-cron</code> — not public.</sub>

## Technical skills

**Languages** &nbsp;
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

**AI & LLM systems** &nbsp;
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square) ![Vercel AI SDK](https://img.shields.io/badge/Vercel%20AI%20SDK-000000?style=flat-square&logo=vercel&logoColor=white) ![OpenRouter](https://img.shields.io/badge/OpenRouter-6467F2?style=flat-square) ![LiteLLM](https://img.shields.io/badge/LiteLLM-2E7D32?style=flat-square)

**Backend & frontend** &nbsp;
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)

**Data & quantitative** &nbsp;
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

**Developer tools** &nbsp;
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white) ![Twilio](https://img.shields.io/badge/Twilio-F22F46?style=flat-square&logo=twilio&logoColor=white)

<br>

<div align="center">

Case studies, architecture notes, and more at <a href="https://yekaiwu.github.io">yekaiwu.github.io</a>

</div>
