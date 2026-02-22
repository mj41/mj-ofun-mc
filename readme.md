# Overview

Umbrella index for all [mj41](https://github.com/mj41)'s Minecraft projects.

Live server: [mc.w42.eu](https://mc.w42.eu)

# Public repos

## go-mc

Public fork with custom branch supporting Minecraft 1.21.11 protocol version.

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
