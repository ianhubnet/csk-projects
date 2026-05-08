# 🧱 CSK Projects

This monorepo hosts all official **applications and projects** built using [CiSkeleton (CSK)](https://github.com/ianhubnet).

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

## ⚙️ Automation

Every project must define:

- `CSK_NAME` variable → name of the project (e.g., `ianhub`).
- `IANHUB_AGENT_CLIENT_ID` and `IANHUB_AGENT_PRIVATE_KEY` → for secure automation communication.

> 🪄 CSK automatically syncs project updates, keeping all related repositories aligned.

---

### Example
| Project | Example Repo | `CSK_NAME` | `IANHUB_AGENT_*` | Added Under |
| :------ | :----------: | :--------: | :--------------: | :---------- |
| `default` | `csk-app-default` | `default` | `<secrets>` | `projects/default` |
| `ianhub` | `csk-app-ianhub` | `ianhub` | `<secrets>` | `projects/ianhub` |
| `example` | `random-app-example` | `example` | `<secrets>` | `projects/example` |

---

> 🧩 The `csk-projects` repo serves as a public index for CSK-powered applications and supports automation around project synchronization and deployment.

## 🌍 Related Repositories

* [`csk-core`](https://github.com/ianhubnet) — Main CSK Framework *(Private)*
* [`csk-common`](https://github.com/ianhubnet/csk-common) — CSK Shared Assets *(Public)*
* [`csk-packages`](https://github.com/ianhubnet/csk-packages) — Modules, plugins, themes, and languages *(Public index)*

---

> This repo acts as an **index** for all CSK-powered applications — some public, most private.

---

## Licensing and Access

This repository acts as a public index for official CSK-powered applications and projects.

The repository itself does not grant usage, deployment, redistribution, or commercial rights to any application referenced here. Each project is governed by its own license, agreement, access policy, or private repository permissions.

Some projects may be private, proprietary, client-specific, or production systems. Public visibility of this index, its folder structure, or its Git submodule references does not imply that the referenced projects are open source or publicly deployable.

Third-party components used by individual projects remain governed by their own respective licenses and should be documented inside the project that directly bundles or distributes them.

---

For licensing questions or additional usage rights, contact: **legal@ianhub.net**
