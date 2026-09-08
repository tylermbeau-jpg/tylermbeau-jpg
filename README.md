# Tyler Beauregard

**Operations leader who ships the systems the team runs on, solo, then deploys them with the people who use them.**

I run finance operations inside a $300M+ public institution and build what it runs on: production apps, agentic pipelines, and the tooling that replaces a spreadsheet nobody trusts. My work lives in the messy last mile: real data, real stakeholders, real production. AI is the multiplier that lets one person ship a full system in days; the judgment about what to build is the operator's job.

## Selected work

- **[District Fiscal Tools](https://districtfiscaltools.com)**: a pre-flight validator for California school-district state filings. It checks every account string against the state's real combination matrices and attaches the corrected string before the state's technical review rejects the file, and it matches the state's own error log on every rule it implements. Launched August 2026 with 100+ published pages explaining each state check; in front of 140+ district fiscal offices in its first week. (Product repo is private; the public rule set below is the same domain.)
- **[school-finance-mcp](https://github.com/tylermbeau-jpg/school-finance-mcp)**: an open-source MCP server (official MCP Python SDK / FastMCP) exposing California school-finance validation and reimbursement tools, built on public CDE data. Deployed live over streamable HTTP: `claude mcp add --transport http school-finance https://school-finance-mcp.onrender.com/mcp` and it is in your agent (free-tier host, so the first call after idle takes a moment).
- **[school-finance-agent](https://github.com/tylermbeau-jpg/school-finance-agent)**: a Claude tool-use agent on top of that server, with a 12-question graded eval suite (mechanical checks: contains, number_close, tool_used). Domain tools to agent to evals, end to end.
- **[claude-hitl-pipeline](https://github.com/tylermbeau-jpg/claude-hitl-pipeline)**: the human-in-the-loop pattern as working code. The model drafts, a person approves or overrides, only approved items execute, and every step lands in an audit log. State machine enforced, fully tested offline.
- **[claude-ops-toolkit](https://github.com/tylermbeau-jpg/claude-ops-toolkit)**: the discipline I run Claude Code with, generalized: planning gates with mechanically checkable acceptance criteria, a hypothesis-driven debugging loop, pre-ship checks, and a report-only QC reviewer agent.
- **[xlsx-recalc](https://github.com/tylermbeau-jpg/xlsx-recalc)**: a small sharp tool for a real pain: openpyxl writes formulas with empty caches, so generated workbooks read blank everywhere except Excel. One command fixes it via LibreOffice headless.
- **[board-agenda-formatter](https://github.com/tylermbeau-jpg/board-agenda-formatter)**: turns a public board-agenda PDF into the condensed internal Word document a district actually circulates. Pure Python, no API key.
- **Executive command center** (private): the 12-page dashboard a $300M+ institution's chief business official runs budget, payroll, position control, and multi-year projections from, fed by Python pipelines over the ERP's ledger and payroll extracts. The shared pacing view behind it lifted operating-budget utilization from 70% to 97%.
- **Data Forge** (private): a live 12-module operations platform (Next.js + FastAPI on Vercel + Render + Supabase) a department runs on daily; automated ingest of six source formats, student data out by design.
- **Position-tracking system** (private): a custom Next.js + Prisma app built to replace a vendor tool after a build-versus-buy call; its validation surfaced 17 personnel misallocations, an estimated ~$1.7M at loaded cost.

## How I build

Scope it with the person who will run it, write the one-page decision doc, ship the working system, hand it off with a runbook and an audit log. A self-built Claude Code stack (skills, review subagents, scheduled jobs; the patterns are in claude-ops-toolkit) plus Claude API pipelines with a human approving anything that matters is how I move at one-person scale.

## Tech

`Python` · `Next.js` · `FastAPI` · `TypeScript` · `Claude API` · `Claude Code` · `MCP` · `Supabase` · `Postgres` · `SQL` · `Vercel` · `Render` · `git`

Founder, Databros LLC · Burbank, CA
