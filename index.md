---
title: Eric Guichard
---

My public repositories: tools I built to run my own household's network, home and notes, published in case they help someone else.

## Egressor

**One YAML manifest, a household's whole egress path out of a hostile network.**

Reliable internet access from inside, or while travelling to, a country with a national firewall (China, Russia, Iran). You describe your users, their devices and their regions in one YAML file; `render.py` produces a per-device [sing-box](https://github.com/SagerNet/sing-box) config for each of them (Android, iOS, Windows, macOS, Linux), a hardened Docker Compose stack for the server, and one-line installers that keep clients up to date.

- Five protocol paths through deep packet inspection (VLESS+Reality, Hysteria2, ShadowTLS, VLESS over a Cloudflare WebSocket, optional AmneziaWG), with a per-region default
- Per-region routing, routine credential rotation with a grace window, optional "home egress" for travellers
- DNS-level threat and ad blocking by default

[Website](https://egressor.org) · [Repository](https://github.com/ericguichard/egressor) · Python · AGPL-3.0

## Flux

**A personal AI assistant built on a second-brain structure.** You capture things into a Discord channel; Claude files, links, summarises, drafts and asks you questions in an Obsidian vault you read on your phone or laptop. Designed as a chief of staff with a strict security badge: the part that reads incoming material cannot send or spend anything.

### Flux vault template

The memory half: an Obsidian vault that Claude maintains using the LLM Wiki pattern. It holds the rules Claude follows, the folder layout, the page template and the daily and weekly briefings, and no content. Press "Use this template" on GitHub for your own private copy.

[Repository](https://github.com/flux-brain/vault-template) · Shell · Apache-2.0

### Flux server

The server half: runs on a small always-on machine and connects the Discord channel to the vault. Captures (text, photos, PDFs, Office files, emails, voice memos) become inbox files, the filing routine starts on its own, and answers, drafts and digests come back to the channel. Optional modules sync Google Tasks and Google Calendar.

[Repository](https://github.com/flux-brain/server) · Python · Apache-2.0

## Sesame for Home Assistant

**Open gates, doors and barriers from Home Assistant.** An integration for a Sesame access-control server: one button per access point the server reports, also reachable from Apple Home and Google Home through Home Assistant's bridges. Buttons go unavailable when a token is revoked, the server is unreachable, an access point is closed for the season or its equipment is offline. Authorisation and logging stay on the server.

[Repository](https://github.com/ericguichard/hass-sesame) · Python · MIT · installable through HACS as a custom repository

## Fork

### hass_nuki_ng

Fork of [kvj/hass_nuki_ng](https://github.com/kvj/hass_nuki_ng), better support for Nuki smart locks in Home Assistant (bridge, cloud API or both). My two commits move it off a device-registry API that Home Assistant deprecated in 2026.10 and removes in 2027.8.

[Repository](https://github.com/ericguichard/hass_nuki_ng) · Python · MIT
