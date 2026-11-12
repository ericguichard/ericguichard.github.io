---
title: Eric Guichard
---

My public repositories: tools I built to run my own notes and assistant, published in case they help someone else.

## Flux

**A personal AI assistant built on a second-brain structure, designed security first: anything goes in, in any form, and comes back at the depth you need, but nothing goes out without you.**

Flux is a chief of staff with a strict security badge. You hand it whatever you have; Claude files it, links it to what it already knows, summarises, drafts and asks you questions. It cannot send or spend anything on its own.

**Security model: whoever opens the post does not sign the cheques.** An assistant that reads your mail is exposed to every message anyone sends you, including forged ones written to manipulate an AI. Flux answers this with separation of duties, the control a finance team uses:

- **The reader cannot act.** The AI that reads incoming material works in a locked room: it sees only the vault repository, with no internet, no email, no connectors and no payment means. A forged letter can say "wire the money", but the one reading it has no access to the bank.
- **Incoming content is data, never instructions.** Emails, attachments, calendar entries and captures are filed and summarised; requests written inside them are never followed, and links in them are never opened by the filing routine.
- **The couriers do not think.** The server programs that carry things in and out run fixed procedures and make no judgement calls.
- **Acting outside needs you in the room.** Anything beyond the vault (sending, changing files in your cloud storage, browsing) happens only in an interactive session that you are attending, and only once you say yes.
- **Least privilege everywhere.** Drive and Calendar access is read-only. The only email Flux sends on its own is the weekly briefing, and only to your own address, read from the account rather than from settings or vault content.
- **Private conversations stay private.** Flux never reads your messaging apps; it only sees the channels you created for it.

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

Optional modules bring Google Tasks and Google Calendar into the same flow: each project's open actions become a Tasks list you can tick and edit on your phone. Coming next: an open-items Google Sheet where you see every open item and can type an instruction on a row.

### Flux vault template

The memory half: an Obsidian vault that Claude maintains using the LLM Wiki pattern. It holds the rules Claude follows, the folder layout, the page template and the daily and weekly briefings, and no content. Press "Use this template" on GitHub for your own private copy.

[Repository](https://github.com/flux-brain/vault-template) · Shell · Apache-2.0

### Flux server

The server half: runs on a small always-on machine and connects the Discord channel to the vault. Every capture becomes an inbox file, the filing routine starts on its own, and answers, drafts and briefings come back to the channel.

[Repository](https://github.com/flux-brain/server) · Python · Apache-2.0
