<div align="center">

# PortBay

### Run every local project like a tiny PaaS — not an unmanaged server.

One Play button per project. Real HTTPS `.test` domains, managed DNS and
reverse proxy, live logs. No containers, no daemon zoo, no hand-edited `/etc/hosts`.

[![License: AGPL-3.0](https://img.shields.io/badge/license-AGPL--3.0-1f6feb.svg)](https://github.com/portbay-app/portbay/blob/main/LICENSE)
[![Platform: macOS](https://img.shields.io/badge/macOS-Apple%20Silicon-black.svg?logo=apple&logoColor=white)](https://github.com/portbay-app/portbay)
![Status: pre-1.0](https://img.shields.io/badge/status-pre--1.0-orange.svg)
[![Stars](https://img.shields.io/github/stars/portbay-app/portbay?style=flat&color=1f6feb)](https://github.com/portbay-app/portbay/stargazers)

**[Get PortBay](https://github.com/portbay-app/portbay)** ·
[Documentation](https://portbay-app.github.io/portbay/) ·
[Discussions](https://github.com/portbay-app/portbay/discussions) ·
[Contribute](https://github.com/portbay-app/portbay/blob/main/CONTRIBUTING.md) ·
[Security](https://github.com/portbay-app/portbay/blob/main/SECURITY.md)

`Tauri 2` · `Rust` · `Svelte 5` · macOS today, Linux & Windows planned

</div>

<!-- TODO: add a hero screenshot or short GIF of the dashboard here — highest-impact
     visual upgrade once a capture exists. Don't ship a broken image link before then. -->

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

- ▶️ **One-click Play / Stop per project** — Next.js, Vite, plain Node, PHP, Laravel.
- 🛑 **A universal Stop-All** that works even after a crash.
- 🔒 **Real HTTPS** like `https://myproject.test`, issued and trusted locally.
- 🌐 **Wildcard `.test` routing** via a bundled DNS resolver — zero hosts-file edits.
- 🧭 **Reverse-proxy routing** managed for you through Caddy's admin API.
- 📜 **Live logs, status, and metrics** per project, plus a macOS menu-bar mode.

Native and small by design — target under ~80 MB idle RAM and a sub-30 MB
installer. The GUI is a thin client over a Rust core with full CLI parity.

## How it fits

|  | PortBay | Laravel Herd | MAMP / XAMPP | Docker / OrbStack |
|---|---|---|---|---|
| Open source | ✅ AGPL-3.0 | ❌ | ❌ | Engine ✅ / app ❌ |
| Container-free | ✅ | ✅ | ✅ | ❌ |
| Local HTTPS + `.test` | ✅ | ✅ | partial | manual |
| Multi-runtime (Node / PHP / …) | ✅ | PHP-first | PHP-first | ✅ |
| Idle footprint | small (native) | small | medium | large |

If you live in PHP on macOS, Herd is excellent. PortBay's bet is one open,
lightweight tool for mixed Node/PHP/static stacks — no container layer, nothing
you couldn't build yourself.

## Editions

| | **PortBay Community** | **PortBay Cloud / Pro** |
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
