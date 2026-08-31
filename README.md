> This repository contains **only** `README.md` layout maps for `~/dev`. No source, backups, or secrets.

# `~/dev`

Software workspace. Everything belongs in one of four roots. Legacy paths are kept as symlinks.

| Path | Role | What belongs here |
| --- | --- | --- |
| `personal/` | Active repos you own (`mamahoos`) | Work in progress, with `.git` |
| `work/` | Employer work | Kept separate from personal |
| `vendor/` | Other people's clones | upstream ≠ mamahoos |
| `studio/` | Non-repo: archive + desk | Knowledge, ops, backups, dead code |

Studio details: [`studio/README.md`](studio/README.md)

## Path compatibility (do not remove)

These names must remain at the root of `~/dev`:

| symlink | Target |
| --- | --- |
| `archive` | `studio/archive` |
| `configs` | `studio/desk/config` |
| `DevOps` | `studio/desk/runbooks` |

Inside archive: `docker-images` → `artifacts/container-images/docker-images`
