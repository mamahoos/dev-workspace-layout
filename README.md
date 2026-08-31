> This repository contains **only** `README.md` layout maps for `~/dev`. No source, backups, or secrets.

# `~/dev`

Software workspace. Six roots; two of them are compatibility names.

| Path | Role | What belongs here |
| --- | --- | --- |
| `personal/` | Active repos you own (`mamahoos`) | Work in progress, with `.git` |
| `work/` | Employer work | Kept separate from personal |
| `vendor/` | Other people's clones | upstream ≠ mamahoos |
| `archive/` | Frozen: dead projects + dumps | Not an active git workspace |
| `desk/` | Live: knowledge + day-to-day ops | Secrets, runbooks, learning |
| `configs` | symlink | `desk/config` |
| `DevOps` | symlink | `desk/runbooks` |

`archive/` is a real directory (the old `archive` → `studio/archive` link is gone). `configs` and `DevOps` must stay.

Inside archive: `docker-images` → `artifacts/container-images/docker-images`

## Where does this file go?

```
new file
  ├─ unknown yet?                         → desk/inbox/
  ├─ secret / key / recovery / SSH        → desk/config/   (never git)
  ├─ "how do I deploy / debug this?"      → desk/runbooks/
  ├─ compose / env / server bundle        → desk/deploy/<service>/
  ├─ incident with time and actions       → desk/incidents/
  ├─ reusable skeleton (seed, compose)    → desk/templates/
  ├─ raw paste for an LLM                 → desk/llm/
  ├─ screenshot / image                   → desk/media/
  ├─ learning / PDF / short reference     → desk/knowledge/
  ├─ dead project / old source tree       → archive/projects/<name>/
  └─ zip, DB dump, docker save, export    → archive/artifacts/…
```

Active git repos → `personal/` or `work/`.

## Naming

- kebab-case; no spaces in directory names
- dated dumps: `YYYY-MM-DD-topic`
- README files describe layout only, not project internals
