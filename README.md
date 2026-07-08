# VibeNest Template: Memos

This is a thin VibeNest-ready deploy adapter for [Memos](https://github.com/usememos/memos).

It does not fork or modify the Memos product. The repository only provides deploy-safe defaults for platforms that deploy from a Git repository:

- official image: `neosmemo/memos:stable`
- app port: `5230`
- persistent data volume: `/var/opt/memos`
- SQLite by default, no external database required

## VibeNest notes

Use this repository when raw upstream deployment is not desired. The upstream repository contains the full application source and optional database drivers, which can lead generic build detection toward the wrong build directory or an unnecessary managed database. This adapter keeps deployment explicit and small.

After first launch, create the first Memos account in the web UI and keep the volume attached for upgrades.

## Upstream

- Product: https://github.com/usememos/memos
- Docs: https://usememos.com/docs/deploy/docker
- Image: https://hub.docker.com/r/neosmemo/memos

