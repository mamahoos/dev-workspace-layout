# `studio/` — non-repo workspace

Two trees, two lifetimes:

```
studio/
  archive/     frozen: dead projects + dumps
  desk/        live: knowledge + day-to-day ops
```

Active git repos do not live here → `~/dev/personal` or `~/dev/work`.

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

## Naming

- kebab-case; no spaces in directory names
- dated dumps: `YYYY-MM-DD-topic`
- README files describe layout only, not project internals

## `~/dev` symlinks

`archive` → here; `configs` → `desk/config`; `DevOps` → `desk/runbooks`.
