# `desk/` — live workbench

Ops and knowledge stay separate:

```
desk/
  config/      secrets and env notes      ← ~/dev/configs
  runbooks/    operational how-to         ← ~/dev/DevOps
  deploy/      compose/env server bundles
  incidents/   postmortems
  knowledge/   learning, PDFs, refs, talks
  templates/   reusable skeletons
  inbox/       intake; empty it
  llm/         raw text for a model
  media/       images
```

Do not commit `config/`. Course PDFs and slides belong in `knowledge/`, not `runbooks/`.
