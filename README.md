# Codium Red — showcase

**Portfolio:** [ahelijao.github.io](https://ahelijao.github.io/) · Chapter VI  
**Private source:** not linked

> Docs-only public view. **No exploits, no lab spoilers, no VPN profiles, no payloads.**

## Elevator

**AI-assisted pentest architecture** with a hard split: an **intelligence plane** (agent plans / structures) and an **isolated execution plane** (containerized tooling). Humans validate — the agent does not replace judgment.

## Need

| Pain | Response |
|------|----------|
| AI and offensive tools on one messy host | Separate control plane vs execution plane |
| Unstructured recon notes | Agent helps organize findings / next steps |
| Scanner sprawl | Dockerized tool services (e.g. proxy/scanner) with a host bridge |

## Architecture (sanitized)

```text
┌────────────────────────────┐
│  Intelligence plane        │
│  Agentic IDE / planner     │
│  reports · methodology     │
└─────────────┬──────────────┘
              │ command / telemetry bridge
              ▼
┌────────────────────────────┐
│  Execution plane (Docker)  │
│  hardened tool containers  │
│  e.g. scanner / proxy API  │
└────────────────────────────┘
```

**Discipline:** demos are supervised lab-style. This public page describes **planes and process**, never weaponized detail.

## What this demonstrates

- Security engineering mindset applied to AI systems
- Isolation as a first-class design constraint
- OWASP-oriented methodology over “AI did a hack”

## Stack

`Python` · `Docker` · PowerShell/shell glue · scanner/proxy services (e.g. ZAP API) · OWASP methodology

## Hard red lines

- No exploit code  
- No machine writeups  
- No credentials or network configs  


## Full source (private)

Access required. The implementation lives in a **private** repository:

- [Codium-Red](https://github.com/AHelijao/Codium-Red)

Without collaborator access, GitHub will show **404**. To request access: email [helijao.andriamandranto@gmail.com](mailto:helijao.andriamandranto@gmail.com), message on [LinkedIn](https://linkedin.com/in/helijaoa), or open an issue on **this** showcase repo — I’ll grant access case by case.

---

← back to [portfolio](https://ahelijao.github.io/) · Helijao Andriamandranto
