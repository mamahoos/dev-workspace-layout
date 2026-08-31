# `artifacts/` — non-source

| Directory | Contents |
| --- | --- |
| `archives/projects/` | zip/tar project snapshots |
| `archives/platforms/` | heavy service/server backups |
| `archives/generic/` | unlabeled tar/zip |
| `exports/` | app exports; keep zip next to `unpacked/` |
| `container-images/docker-images/` | `docker save` output |
| `databases/` | standalone `.sql` / `.db` (not `.db` inside a repo) |
| `documents/` | one-off documents that are not a project |
| `scripts/` | stray sh/py |
| `config-snippets/` | config fragments; `vpn/` is sensitive |

Compatibility path: `archive/docker-images` → `container-images/docker-images`.
