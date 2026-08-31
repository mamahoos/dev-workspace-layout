# How I keep `~/dev` sorted

This is not an application. It is the map of **the main code directory on my machine**: `~/dev`.

That folder holds everything I build and keep: active git repos, clones of other people's work, frozen projects, notes, runbooks, dumps. It got messy. Finding a home for a new file was guesswork.

I split it into a few roots, put a short `README.md` in each, and use those files as the rule. **This repository is that map, shared.** The real trees — source, backups, secrets — stay on disk. They are not in git.

If you are reading this on GitHub, you are looking at the labels on empty shelves, not the shelves' contents.

## Roots

| Path | Role |
| --- | --- |
| `personal/` | My active repos (`mamahoos`) |
| `work/` | Employer work, kept separate |
| `vendor/` | Other people's clones |
| `archive/` | Frozen projects and dumps |
| `desk/` | Live notes, ops, learning |
| `configs` | symlink → `desk/config` |
| `DevOps` | symlink → `desk/runbooks` |

`archive/` is a real directory. `configs` and `DevOps` must stay; old habits and scripts still use those names.

Inside archive: `docker-images` → `artifacts/container-images/docker-images`

## Where does a new file go?

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

Deeper rules live next to each folder in this repo (`archive/`, `desk/`, …).
