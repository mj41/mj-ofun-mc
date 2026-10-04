# Overview

Umbrella index for all [mj41](https://github.com/mj41)'s Minecraft projects.

Live server: [mc.w42.eu](https://mc.w42.eu)

Other projects: [mj-ofun](https://github.com/mj41/mj-ofun).

# Public repos

## mc26, go-mc26, go-mc26-kit, mc26-data, mc26-data-pre

A Go library for Minecraft: Java Edition 26.x, generated from Mojang's unobfuscated server jars: the network protocol, game data and world formats as Go types, one branch per Minecraft version (26.1, 26.2, 26.3). Not a fork: a new Minecraft version means "extract, generate, build", and the compiler points at what changed. License: MIT.

```
Mojang jar ──► mc26 ──┬─► mc26-data      (releases)                ──► mc26 ──► go-mc26     (the library)
                      └─► mc26-data-pre  (snapshots, pre-releases)                ◄── go-mc26-kit (bot, server, accounts, examples)
```

git repos:
- [mc26](https://github.com/mj41/mc26): the extractors (jar → JSON), the generators and the `mc26` pipeline command
- [go-mc26](https://github.com/mj41/go-mc26): the generated library, `mc-<version>` branches, tags `v0.<YYN>.<patch>` (`v0.263.0` is Minecraft 26.3)
- [go-mc26-kit](https://github.com/mj41/go-mc26-kit): a client, a server framework, account flows and examples, built against every supported library version
- [mc26-data](https://github.com/mj41/mc26-data): the game data and typed wire schema of every release as JSON, with Markdown docs
- [mc26-data-pre](https://github.com/mj41/mc26-data-pre): the same for snapshots and pre-releases

## go-mc

The older approach: a public fork of [Tnze/go-mc](https://github.com/Tnze/go-mc) with custom branch `mj-262-cubes` supporting Minecraft 26.2 (protocol 776); `mj-121-cubes` is the frozen 1.21.11 line. go-mc26 above is its successor.

git repo: [go-mc](https://github.com/mj41/go-mc) (public fork)

## minecraft-fedora-installer

Minecraft Java Edition installer/launcher helper for Fedora Linux.

git repo: [minecraft-fedora-installer](https://github.com/mj41/minecraft-fedora-installer) (public)

# Private repos

Interested in Minecraft, Go, and Kubernetes? Let me know if you want access to any of these repos. I'm also looking for collaborators on the "Cubes in Motion" project and welcome [sponsors](https://github.com/sponsors/mj41).

## w42-mc-cubes

Survival multiplayer server where each player owns an isolated 512×512 cube world separated by barriers. Players build in their home cube (Survival mode), visit neighbors (Adventure mode), and experience periodic cube rotation that randomizes the entire neighborhood. Claim new free cubes by placing a bed, or quest in dedicated quest cubes that reset overnight. Tunnels enable cube-to-cube travel between adjacent cubes; gates support long-distance portals.

git repo: [w42-mc-cubes](https://github.com/mj41/w42-mc-cubes) (private)

## w42-mc-web

Website for [mc.w42.eu](https://mc.w42.eu) — the web portal for the Cubes in Motion Minecraft server.

git repo: [w42-mc-web](https://github.com/mj41/w42-mc-web) (private)

### Sponsorship

Support the "Cubes in Motion" Minecraft server. Help us build a vision of safe home cubes where you can build and chill, with various cube types to enjoy fun and adventure with friends. Monthly contributions help sustain the server and fund ongoing development.

- **Minecraft**: [Patreon - Minecraft tier](https://www.patreon.com/15562538/join)
- **General support**: [GitHub Sponsors - mj41](https://github.com/sponsors/mj41)

## w42-mc-cubes-plugin

Spigot/Paper plugin for the Cubes game mode.

## w42-mc-server-img

Builds the `cubes-minecraft` container image using a two-stage `Containerfile`: stage 1 pre-downloads the Paper JAR (cached via GHA BuildKit), stage 2 adds the plugin + init data.

git repo: [w42-mc-server-img](https://github.com/mj41/w42-mc-server-img) (private)

## w42-mc-rotate-img

Builds the `cubes-rotation-worker` container image: the world generation and rotation tools from `w42-mc-cubes`, for the periodic cube rotation.

git repo: [w42-mc-rotate-img](https://github.com/mj41/w42-mc-rotate-img) (private)

## w42-mc-cubes-init

Reference world data for cubes server initialization container (cloned at pod startup).

git repo: [w42-mc-cubes-init](https://github.com/mj41/w42-mc-cubes-init) (private)

## w42-mc-cubes-tmpls

Repository of pregenerated cubes used as templates for new cube assignments.

git repo: [w42-mc-cubes-tmpls](https://github.com/mj41/w42-mc-cubes-tmpls) (private)

## w42-mc-backup

`mc-backup-controller` — Go-based Kubernetes controller for automated Minecraft world backups via git.

git repo: [w42-mc-backup](https://github.com/mj41/w42-mc-backup) (private)

## w42-mc-dev

Local development and testing environment for Minecraft on kind. Includes Tiltfile, Go test harness, and local backup testing.

git repo: [w42-mc-dev](https://github.com/mj41/w42-mc-dev) (private)

## w42-mc-world-saves

Local collection of Minecraft world saves for testing and reference. Includes flat worlds and other test worlds.

## mj41-linode

Infrastructure GitOps repository with Kustomize manifests for LKE cluster (Flux CD). Hosts cubes server overlay.

git repo: [mj41-linode](https://github.com/mj41/mj41-linode) (private)

## w42-bck-cubes

git repo: [w42-bck-cubes](https://github.com/mj41/w42-bck-cubes) (private)
