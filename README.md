## Hi 👋 — I'm Sahil

CTO of [Noon](https://noon.design). On the side, I'm building open-source AI tooling for developers and designers. We use these daily at Noon.

Small Go CLIs that compose into a **Complete AI Coding Workflow**:

```txt
spec → parallel agent sessions → ship
```

No SDK, no vendor lock-in, no opinions you can't override.

This page ([ai.shll.in](https://ai.shll.in)) is the canonical home for everything below.

### Install everything

```bash
brew install sahil87/tap/all   # installs every tool in the toolkit
shll shell-install             # one command to wire shell integration into your rc file
exec $SHELL                    # reload so the integration takes effect
```

Later, `shll update` upgrades every installed tool in one go. See the [shll README](https://github.com/sahil87/shll) for the full command surface.

### How the tools fit together

The toolkit is a workflow, not a buffet — though each tool stands alone.

```
Workflow:  idea ──► fab-kit ──► wt ──► run-kit
           (backlog) (pipeline) (worktrees) (tmux dashboard)

Helpers:   hop  · cross-repo navigation
           tu   · cost tracking
           shll · install/update glue
```

You capture an idea with `idea`, turn it into a structured change with `fab-kit`, isolate it in a `wt` worktree so you can run several in parallel, watch them all from `run-kit`'s browser dashboard, `hop` between repos when the work crosses boundaries, and check what it's costing you with `tu`. `shll` keeps everything installed and updated.

### Tools

| Tool | One-liner |
|------|-----------|
| [**fab-kit**](https://github.com/sahil87/fab-kit) | 7-stage pipeline that forces AI agents to plan before they code. Works with Claude Code, Codex, Cursor, Windsurf. |
| [**wt**](https://github.com/sahil87/wt) | Opinionated `git worktree` wrapper — one worktree per change, one AI session per worktree, zero conflicts. |
| [**idea**](https://github.com/sahil87/idea) | Plain-Markdown backlog (`fab/backlog.md`) — worktree-aware, queryable from the CLI, feeds `/fab-new`. |
| [**run-kit**](https://github.com/sahil87/run-kit) | Browser dashboard for tmux + Claude Code workspaces. Mobile-friendly via Tailscale. |
| [**hop**](https://github.com/sahil87/hop) | Fuzzy-nav, batch-git, and run-anything-inside-any-repo from one `hop.yaml` config. |
| [**tu**](https://github.com/sahil87/tu) | Token/cost tracker for Claude Code, Codex, OpenCode. Multi-machine sync, live watch mode. |
| [**shll**](https://github.com/sahil87/shll) | Meta-CLI — `shll install / update / shell-install` to wire and maintain the whole toolkit. |

### Install individually

Or pick individual formulas from [`sahil87/homebrew-tap`](https://github.com/sahil87/homebrew-tap):

```bash
brew install sahil87/tap/<formula>
```

### Community

Questions, feature requests, or just want to chat about AI dev tooling? **[Join the Discord](https://discord.gg/32XHh5mJYn)** — that's where I answer queries, share what I'm building, and discuss with people using these tools.

### Find me

[LinkedIn](https://in.linkedin.com/in/ahujasahil) · [X](https://x.com/_sahilahuja) · [Discord](https://discord.gg/32XHh5mJYn) · [ai.shll.in](https://ai.shll.in)
