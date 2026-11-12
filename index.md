---
title: Eric Guichard
---

My public repositories: tools I built to run my own notes and assistant, published in case they help someone else.

## Flux

**A personal AI assistant built on a second-brain structure: anything goes in, in any form, and comes back at the depth you need.**

Flux is a chief of staff with a strict security badge. You hand it whatever you have; Claude files it, links it to what it already knows, summarises, drafts and asks you questions. The part that reads incoming material cannot send or spend anything.

**Multi-modal in.** One Discord channel takes everything, from any device:

- typed notes and questions
- voice memos
- photos and screenshots
- PDFs and Office files
- forwarded emails

**Multi-level out.** The same knowledge reaches you at the level of detail the moment calls for:

1. **A glance:** a short answer or a question back in the Discord channel, on your phone.
2. **A briefing:** "Your day ahead" every morning and "Your week ahead" on Sundays.
3. **A page:** one Obsidian page per project, person or topic, kept current and linked to the others, readable on phone or laptop.
4. **The source:** every original capture is kept and filed, so any summary can be traced back to what it came from.

Optional modules bring Google Tasks and Google Calendar into the same flow.

### Flux vault template

The memory half: an Obsidian vault that Claude maintains using the LLM Wiki pattern. It holds the rules Claude follows, the folder layout, the page template and the daily and weekly briefings, and no content. Press "Use this template" on GitHub for your own private copy.

[Repository](https://github.com/flux-brain/vault-template) · Shell · Apache-2.0

### Flux server

The server half: runs on a small always-on machine and connects the Discord channel to the vault. Every capture becomes an inbox file, the filing routine starts on its own, and answers, drafts and briefings come back to the channel.

[Repository](https://github.com/flux-brain/server) · Python · Apache-2.0
