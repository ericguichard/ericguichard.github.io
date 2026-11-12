---
title: Eric Guichard
---

My public repositories: tools I built to run my own notes and assistant, published in case they help someone else.

## Flux

**A personal AI assistant built on a second-brain structure.** You capture things into a Discord channel; Claude files, links, summarises, drafts and asks you questions in an Obsidian vault you read on your phone or laptop. Designed as a chief of staff with a strict security badge: the part that reads incoming material cannot send or spend anything.

### Flux vault template

The memory half: an Obsidian vault that Claude maintains using the LLM Wiki pattern. It holds the rules Claude follows, the folder layout, the page template and the daily and weekly briefings, and no content. Press "Use this template" on GitHub for your own private copy.

[Repository](https://github.com/flux-brain/vault-template) · Shell · Apache-2.0

### Flux server

The server half: runs on a small always-on machine and connects the Discord channel to the vault. Captures (text, photos, PDFs, Office files, emails, voice memos) become inbox files, the filing routine starts on its own, and answers, drafts and digests come back to the channel. Optional modules sync Google Tasks and Google Calendar.

[Repository](https://github.com/flux-brain/server) · Python · Apache-2.0
