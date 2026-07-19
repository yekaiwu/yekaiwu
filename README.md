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

<img src="assets/realtor-os-workflows.png" width="100%" alt="Diagram of Realtor OS's versioned workflow compiler: a prompt version, workflow stages, and runtime variables render into a compiled system prompt pinned to each conversation">
<sub>System diagram: versioned prompt compiler.</sub>

### Realtor OS

A lead-engagement operating desk for property agents — inbound WhatsApp and voice leads, assistant-led qualification, bookings, inventory, and CRM sync in one runtime. A workflow compiler renders a versioned prompt, workflow definition, and runtime variables into a system prompt and tool set, pinning each live conversation to its own version so a thread never shifts mid-edit; the stack runs fully offline against a local JSON store and deterministic mock providers, covered by Vitest unit, smoke, readiness, and route-level E2E suites.

<code>Next.js</code> <code>Vercel AI SDK</code> <code>Twilio</code> <code>Postgres</code> <code>Twenty CRM</code>

</td>
<td width="50%" valign="top">

<img src="assets/jump-cup-brier.png" width="100%" alt="Diagram of Jump Cup's forecasting pipeline: a question parser fans out into 8 model families, ensembles their outputs, then applies isotonic calibration gated against crowd Brier score">
<sub>System diagram: calibrated ensemble pipeline.</sub>

### Jump Cup

A multi-model probability-forecasting engine for World Cup markets, built around Brier-score calibration rather than confident winner picks. A question parser (LLM plus heuristic, cross-checked) routes into 8 model families, ensembles their outputs, then applies isotonic calibration and base-rate shrinkage; a calibration gate fails the build unless the engine's Brier score beats crowd consensus across 198 settled markets from 20 captured matches.

<code>Python</code> <code>scikit-learn</code> <code>OpenRouter</code> <code>SQLite</code>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<img src="assets/chess-coach.png" width="100%" alt="Diagram of Chess Coach's backend pipeline: Stockfish position analysis feeds win-probability and centipawn scoring into a LangChain chat layer routed to commentary, tactics, and chat endpoints">
<sub>System diagram: engine-grounded coaching pipeline.</sub>

### [Chess Coach ↗](https://github.com/yekaiwu/Chess_Coach)

A full-stack chess coach that turns Stockfish evaluations into contextual commentary, tactics, and a coaching chatbot. A FastAPI backend coordinates Stockfish analysis with LangChain-based chat, exposing evaluation, commentary, tactics, and chat as separate routes consumed by a React/TypeScript client, delivered through a Dockerized local setup with separate backend, frontend, and integration CI workflows plus a scheduled security scan.

<code>React</code> <code>TypeScript</code> <code>FastAPI</code> <code>Stockfish</code> <code>LangChain</code>

</td>
<td width="50%" valign="top">

<img src="assets/job-app-pipeline.png" width="100%" alt="Diagram of Job App's pipeline: discover, filter, tailor, and fill stages, with a three-way KNOWN, INFERABLE, and PERSONAL-UNKNOWN field-routing split before a DRY_RUN-gated submit">
<sub>System diagram: field-routed application pipeline.</sub>

### Job App

An autonomous job-search pipeline that discovers roles from public ATS boards, filters them for relevance and eligibility, tailors resume bullet points per role via an LLM, and fills applications through a Playwright browser session. Every form field routes to KNOWN (candidate database), INFERABLE (LLM-written), or PERSONAL-UNKNOWN — surfaced once and reused forever — so it never guesses a personal fact, with a `DRY_RUN` flag and a human-confirmed submit step keeping it safe to test.

<code>FastAPI</code> <code>SQLModel</code> <code>Playwright</code> <code>React</code>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<img src="assets/mrt-bus-router.png" width="100%" alt="Diagram of the MRT and Bus Router's multi-modal route search from origin to destination with bus, MRT, and walking legs, plus a 42-win/29-tie/29-loss benchmark against Google Maps">
<sub>System diagram: route search and benchmark.</sub>

### [MRT + Bus Router ↗](https://github.com/yekaiwu/mrt-bus)

"Leave now" Singapore transit routing over a custom bounded multi-modal search — live LTA bus arrivals, GTFS rail topology, and OneMap walking data — with zero third-party runtime dependencies. A priority-queue label search applies transfer penalties and same-mode vs. cross-mode walking caps, bounded to 1,500 search labels to keep live LTA quota usage predictable, and benchmarks against the Google Maps Routes API on 100 checkpointed cases: 42 wins, 29 ties, 29 losses, average +1.1 minutes.

<code>Python (stdlib)</code>

</td>
<td width="50%" valign="top">

<img src="assets/nus-tennis-booker.png" width="100%" alt="Diagram of NUS Tennis Booker's race timeline: pre-warm, window open, slot polling every 200ms, slot claimed, and Telegram handoff">
<sub>System diagram: slot-release race timeline.</sub>

### [NUS Tennis Booker ↗](https://github.com/yekaiwu/nus_tennis)

Playwright automation that races a university tennis-court booking portal the instant slots release, then hands the payment step to a human over Telegram. It pre-warms and parks an authenticated session ahead of the release window, polls the slot grid every 200ms once it opens, and runs a separate scheduled health-check job that re-authenticates and asserts the slot grid's DOM hasn't changed, alerting over Telegram if the site breaks.

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
