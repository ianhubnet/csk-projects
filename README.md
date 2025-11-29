# 🧱 CSK Projects

This monorepo hosts all official **applications and projects** built using [CodeIgniter Skeleton (CSK)](https://github.com/ianhubnet).

Each application is developed as a **standalone CSK app**, managed as a **Git submodule** for independent lifecycle and deployment.

## 🧭 Purpose

* Keep all CSK-based applications organized.
* Enable CI/CD automation for production-ready deployments.
* Provide a visible overview of projects under active development.

## 📦 Structure

Projects follow the convention: `csk-app-<example>` and automatically integrate into:

```
projects/
├── default/
├── example/
└── ...
```

## Automation
Every project must define:
- `CSK_STRIP` → prefix to remove (`csk-app-`).
- `CSK_PAT` → personal access token for updates.

> 🪄 CSK automatically syncs project updates, keeping all related repositories aligned.

---

## Example
| Project | Example Repo | CSK_STRIP | CSK_PAT | Added Under |
|---------|--------------|-----------|---------|-------------|
| `default` | `csk-app-default` | `csk-app-` | `<secret>` | `projects/default` |
| `ianhub` | `csk-app-ianhub` | `csk-app-` | `<secret>` | `projects/ianhub` |
| `example` | `random-app-example` | `random-app-` | `<secret>` | `projects/example` |

---

> 🧩 The `csk-projects` repo serves as the foundation for multi-app distribution and deployment.

## 🌍 Related Repositories

* [`csk-core`](https://github.com/ianhubnet) — Core framework *(Private)*
* [`csk-packages`](https://github.com/ianhubnet/csk-packages) — Modules, plugins, and themes *(Public index)*

---

> This repo acts as an **index** for all CSK-powered applications — some public, most private.
