# James Van Daele — Cleburne, Texas

I run a watch & jewelry shop in Cleburne, Texas, and I build software in the
margins around it. The through-line in everything I build is **trust
infrastructure** — I've been scammed and messed over enough times that I
build systems where a customer *can't* easily be messed over.

## What I've built and shipped

- **[dfwmetro.net](https://dfwmetro.net)** — a Dallas–Fort Worth directory of
  genuinely online-bookable service businesses, with a verification desk
  (license, registration, insurance checked before a business gets the
  verified badge). Its MCP server is live and listed in the official MCP
  Registry as `io.github.cexplayer01/dfwmetro-directory`.
  The open-source stdio bridge is here: **[dfwmetro-mcp](https://github.com/cexplayer01/dfwmetro-mcp)** (MIT).
- **[Primed Harness](https://boundedagentharness.com)** (Bounded Agent
  Harness) — governance for long-running AI agent work: budgets set up
  front, explicit authorization for irreversible steps, cost known before
  a run starts, continuation/resume when a run hits a wall, and an audit
  trail of what actually happened.
- **USB** — white-label websites for local businesses ($20 down + $5/mo),
  built so each site doubles as a pre-verified directory listing with
  booking. Status page runs on GitHub Actions:
  [usb-status](https://github.com/cexplayer01/usb-status).
- **[entropy-dice](https://github.com/cexplayer01/entropy-dice)** — random
  numbers for AI that never come from the model: layered, publicly
  verifiable noise (NIST beacon, drand, Bitcoin block hashes, live
  weather, timing jitter) conditioned through SHA-256.
- **[texas-pmtiles](https://github.com/cexplayer01/texas-pmtiles)** — a
  self-hosted basemap of Texas as a single 562 MB PMTiles file, so a map
  product never dies because a free tile service changed its terms.

## What I'm useful for

Hard-won, documented lessons from shipping this stack solo:

- MCP servers: registry listing, stdio ↔ Streamable HTTP bridging,
  keeping tool definitions live-synced instead of copy-pasted.
- AI agent harnesses: per-agent governance adapters, budget ceilings with
  mid-run polls, verification at the layer where the behavior actually
  lives (not where the report says it lives).
- Supabase/Netlify traps: shared-project auth emails falling back to the
  wrong product's domain, deploy manifests silently dropping live files,
  and why I diff every production deploy before/after.
- Programmatic-first workflows: scripts, CLIs and free agent routes doing
  the volume; expensive model tokens reserved for judgment calls.

## How I show up in other people's repos

I don't fork-and-forget. When I fork, it's because I'm bringing a fix or a
feature I needed myself and proved on my own stack first — with tests,
and a short note on where the problem bit me in production.

## Elsewhere

- Directory / MCP: https://dfwmetro.net
- Harness: https://boundedagentharness.com
- Shop: Van Daele Watch & Jewelry, Cleburne TX
