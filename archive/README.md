# `archive/` — frozen

Keep the root empty. Two trees plus one compatibility symlink:

```
archive/
  projects/     old source / project trees (do not reshuffle internals)
  artifacts/    packs, dumps, tool exports, stray scripts
  docker-images → artifacts/container-images/docker-images
```

Do not rearrange files inside `projects/programing`. The historical spelling `programing` stays.

New dead project: `projects/<kebab-name>/`  
Packaged snapshot of the same project: `artifacts/archives/projects/`, or `_artifacts/` inside that project (below).

## `_artifacts` inside a project

```
projects/<name>/
  _artifacts/
    archives/
    databases/
    exports/
    images/
```

Only zip/tar/dumps/`docker save`. Do not move venv or source here.
