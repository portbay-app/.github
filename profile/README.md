<div align="center">

<h1>
  <img src="https://raw.githubusercontent.com/portbay-app/portbay/main/src/lib/assets/portbay-logo.png" alt="" height="112" valign="middle" />
  &nbsp;PortBay
</h1>

### Run every local project like a tiny PaaS — not an unmanaged server.

One Play button per project. Real HTTPS `.test` domains, managed DNS and
reverse proxy, live logs. No containers, no daemon zoo, no hand-edited `/etc/hosts`.

And a task board your AI agents work: write a card, move it to *To Do*, and
Claude Code, Codex, Cursor, or Gemini does the work in your repo.

[![License: AGPL-3.0](https://img.shields.io/badge/license-AGPL--3.0-1f6feb.svg)](https://github.com/portbay-app/portbay/blob/main/LICENSE)
[![Platform: macOS](https://img.shields.io/badge/macOS-Apple%20Silicon-black.svg?logo=apple&logoColor=white)](https://github.com/portbay-app/portbay)
![Status: released](https://img.shields.io/badge/status-released-1f6feb.svg)
[![Stars](https://img.shields.io/github/stars/portbay-app/portbay?style=flat&color=1f6feb)](https://github.com/portbay-app/portbay/stargazers)

**[Get PortBay](https://github.com/portbay-app/portbay)** ·
[Documentation](https://docs.portbay.app) ·
[Discussions](https://github.com/portbay-app/portbay/discussions) ·
[Contribute](https://github.com/portbay-app/portbay/blob/main/CONTRIBUTING.md) ·
[Security](https://github.com/portbay-app/portbay/blob/main/SECURITY.md)

`Tauri 2` · `Rust` · `Svelte 5` · macOS today, Linux & Windows planned

</div>

<div align="center">

<a href="https://try.portbay.app"><img src="https://docs.portbay.app/screenshots/projects-dark.png" alt="PortBay managing local projects" width="840" /></a>

<sub><b><a href="https://try.portbay.app">▶ Try it in your browser</a></b> — the real interface with sample projects, no install required.</sub>

</div>

---

## The problem

Run more than one project locally and your machine becomes a server you never
agreed to administer: background `dev` processes you forgot to kill, ports that
collide, `/etc/hosts` edited by hand, self-signed certs the browser hates, and a
reverse proxy to babysit — times every project you own.

**PortBay owns all of that.** Each project is a declarative record — a hostname,
a start command, a port — and the app reconciles reality to match. Stop the app
and everything stops. Restart one project and the others don't notice.

## What you can do

- 📂 **Point it at a folder — it already knows the project.** PortBay reads the framework (Next.js, Vite, Node, PHP, Laravel) and fills in the start command, port, hostname, and HTTPS. Nothing to configure before the first run.
- ▶️ **One-click Play / Stop per project** — Next.js, Vite, plain Node, PHP, Laravel.
- 🛑 **A universal Stop-All** that works even after a crash.
- 🔒 **Real HTTPS** like `https://myproject.test`, issued and trusted locally.
- 🌐 **Wildcard `.test` routing** via a bundled DNS resolver — zero hosts-file edits.
- 🧭 **Reverse-proxy routing** managed for you through Caddy's admin API.
- 🧪 **A sandboxed runner** — run an untrusted or freshly-cloned project inside a macOS sandbox, inspect it, then promote it to a normal local run.
- 🤖 **An MCP server** — drive your whole local stack from Claude Code, Cursor, or Zed; PortBay's projects and actions become 69 agent tools.
- 🗂️ **A task board your AI agents work** — every project gets a Kanban board; cards are Markdown in your repo. Move one to *To Do* and the agent you assigned does the work and leaves a handoff for the next run.
- 🖥️ **A built-in SSH workspace** — saved hosts, an interactive terminal, an SFTP file browser with inline editing, and port-forward tunnels for the servers your projects ship to.
- 📜 **Live logs, status, and metrics** per project, plus a macOS menu-bar mode.
- 📦 **Already on Herd, ServBay, or MAMP?** Import your existing sites in one step.

Native and small by design — target under ~80 MB idle RAM and a sub-30 MB
installer. The GUI — and your AI agent — are thin clients over a Rust core with
full CLI parity.

## Your agents work the board

Working with a coding agent is still a part-time job: explain the task, watch
it run, repeat — and the context dies with the session. In PortBay you write a
card instead. Move it to **To Do** and the agent you assigned picks it up, does
the work on your machine, and appends a handoff brief the next run reads first.
PortBay launches the coding agents you already have installed — Claude Code,
Codex, Cursor, Gemini, Aider, Copilot, and more — it never runs a model of its own.

<div align="center">

<img src="https://docs.portbay.app/screenshots/tasks-dark.png" alt="PortBay's per-project task board with AI agents working the cards" width="840" />

<sub>One board per project. Cards are Markdown files in the repo — they version with your code.</sub>

</div>

## How it fits

|  | PortBay | Laravel Herd | MAMP / XAMPP | Docker / OrbStack |
|---|---|---|---|---|
| Open source | ✅ AGPL-3.0 | ❌ | ❌ | Engine ✅ / app ❌ |
| Container-free | ✅ | ✅ | ✅ | ❌ |
| Local HTTPS + `.test` | ✅ | ✅ | partial | manual |
| Multi-runtime (Node / PHP / …) | ✅ | PHP-first | PHP-first | ✅ |
| MCP server for agents | ✅ 69 tools | ✅ | ❌ | ✅ |
| AI agent task board | ✅ | ❌ | ❌ | ❌ |
| Agent handoff memory between runs | ✅ | ❌ | ❌ | ❌ |
| Built-in SSH / SFTP / tunnels | ✅ | ❌ | ❌ | ❌ |
| Idle footprint | small (native) | small | medium | large |

If you live in PHP on macOS, Herd is excellent. PortBay's bet is one open,
lightweight tool for mixed Node/PHP/static stacks — where the agent doesn't
just inspect your environment, it picks up the next card and works it.

## Editions

| | **PortBay Community** | **PortBay Pro** |
|---|---|---|
| What | The local-first app — everything above | Optional hosted & team features |
| Where | open source, this org | developed separately |
| License | AGPL-3.0-only | commercial |
| Adds | — | multi-device sync, team workspaces, cloud backups, remote tunnels, org controls *(planned)* |

Community is fully usable offline with no account, and is never crippled to
upsell Pro. *Features marked planned are not built yet.*

## Repositories

- **[portbay](https://github.com/portbay-app/portbay)** — the open-source Community app (AGPL-3.0). **Start here.**

## Get involved

PortBay is early and open — the best time to shape it.

- ⭐ **Star** [portbay](https://github.com/portbay-app/portbay); it genuinely helps it reach other developers.
- 💬 **Ask & propose** in [Discussions](https://github.com/portbay-app/portbay/discussions).
- 🐛 **File bugs / ideas** via [issues](https://github.com/portbay-app/portbay/issues) (templates guide you).
- 🔧 **Send a PR — and earn it back.** A merged *qualifying* pull request grants a
  **perpetual Pro license** tied to your GitHub account. Pay with code, not money.
- 🔒 **Security issue?** Report privately per [SECURITY.md](https://github.com/portbay-app/portbay/blob/main/SECURITY.md) — never a public issue.

New here? Read [CONTRIBUTING.md](https://github.com/portbay-app/portbay/blob/main/CONTRIBUTING.md),
sign off your commits (`git commit -s`), and look for **good first issue** labels.

<div align="center">

---

Built in the open · [portbay.app](https://portbay.app)

</div>
