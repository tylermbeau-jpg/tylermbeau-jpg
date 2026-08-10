# Tyler Beauregard

**Forward Deployed Engineer · Ships production software solo, deploys it with the customer**

I build full-stack and agentic systems end to end, then sit with the non-technical team that has to use them. My work lives in the messy last mile: real data, real stakeholders, real production. AI is the multiplier that lets me ship full systems solo, in days.

## Selected work

- **[school-finance-mcp](https://github.com/tylermbeau-jpg/school-finance-mcp)**: an open-source MCP server (official MCP Python SDK / FastMCP) exposing California school-finance validation and reimbursement tools. Deployed live over streamable HTTP: `claude mcp add --transport http school-finance https://school-finance-mcp.onrender.com/mcp` and it is in your agent.
- **[school-finance-agent](https://github.com/tylermbeau-jpg/school-finance-agent)**: a Claude tool-use agent on top of that server, with a 12-question graded eval suite (mechanical checks: contains, number_close, tool_used). The full stack, domain tools to agent to evals, built end to end.
- **[claude-hitl-pipeline](https://github.com/tylermbeau-jpg/claude-hitl-pipeline)**: human-in-the-loop pattern as working code. The model drafts, a human approves or overrides, only approved items execute, and every step lands in an audit log. State machine enforced, fully tested offline.
- **[claude-ops-toolkit](https://github.com/tylermbeau-jpg/claude-ops-toolkit)**: the discipline structure I run Claude Code with, generalized: planning gates with mechanically checkable acceptance criteria, a hypothesis-driven debugging loop, pre-ship checks, and a report-only QC reviewer agent.
- **[xlsx-recalc](https://github.com/tylermbeau-jpg/xlsx-recalc)**: small sharp tool for a real pain: openpyxl writes formulas with empty caches, so generated workbooks read blank everywhere except Excel. One command fixes it via LibreOffice headless.
- **Data Forge**: a live K-12 financial-operations platform (Next.js + FastAPI on Vercel + Render + Supabase) serving a $300M+ institution. Architected and shipped solo.
- **Position-tracking system**: a custom Next.js + Prisma app built to replace a vendor tool. Its validation surfaced 17 personnel misallocations, a correction on the order of $1.7M.

## How I build

Full-stack apps, agentic pipelines, and the deployment work to put them in front of users. A self-built Claude Code stack (skills, review subagents, scheduled jobs, the patterns in claude-ops-toolkit) plus Claude API pipelines with human-in-the-loop are how I move at one-person scale.

## Tech

`Next.js` · `FastAPI` · `TypeScript` · `Python` · `Claude API` · `Claude Code` · `MCP` · `Vercel` · `Render` · `Supabase` · `SQL` · `git`

Founder, Databros LLC.
