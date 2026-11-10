# easy-for-them

**When a person has to do something, make it almost effortless.**

`easy-for-them` is an agent skill for Claude Code (and any agent that reads `SKILL.md` skills). Agents love to answer with "go to Settings, then Billing, then Accounts, then...". Busy people, and especially your clients on a phone, get lost and give up. `easy-for-them` makes the agent remove every step it can, give direct links that land on the exact screen, write one action per line in plain words, and hand you a message ready to forward to your client as-is.

## See the difference

> **You:** Tell my client how to give us admin access to their page.

**Without the skill:** a paragraph that says "go to settings and look for the permissions section". The client gets lost and calls you.

**With the skill:** a message ready to forward: a direct link to the exact screen, one action per line, plain words, and what they will see when it worked.

**Skip it if** the reader is a developer who prefers reference docs.

**Status:** in daily use in the author's own setup. Plain instructions, no scripts, no network calls. MIT. Issues and suggestions welcome.

## What it does

| Problem | How easy-for-them fixes it |
|---|---|
| "Go to Settings > Billing > ..." | A direct link to the exact screen, with the IDs already in it |
| Asking for things the agent could read | It reads them itself and asks only for the rest |
| Long technical tutorials | One action per line, plain words, sized for a phone |
| "Tell your client to..." | A message written in your voice, ready to copy and send |
| "Did it work?" | It says what success looks like and checks it |

## Install

With the [skills CLI](https://skills.sh):

```bash
npx skills add RabbitDesigns22/easy-for-them
```

Or manually: copy `skills/easy-for-them/` into `~/.claude/skills/` for all your projects, or into `.claude/skills/` for one project.

To make every session use it, add this line to your `CLAUDE.md`:

```
Before writing instructions or a message someone else has to follow, load the easy-for-them skill.
```

## Works well with

- [`hands-on`](https://github.com/RabbitDesigns22/hands-on): the agent does every step it can; this skill covers the steps only a person can do.
- [`one-answer`](https://github.com/RabbitDesigns22/one-answer): one checked, final answer.

## Español

**Pónselo fácil a la gente.** Cuando alguien tiene que hacer algo (tú o tu cliente), el agente quita todos los pasos que puede, da el enlace directo a la pantalla exacta, escribe una acción por línea en palabras simples y te deja el mensaje listo para reenviarle a tu cliente tal cual, con tu voz. Nada de "entra a Configuración, luego a Facturación...".

Instalar: `npx skills add RabbitDesigns22/easy-for-them`

## More skills from the same setup

These come from one real workflow: a small agency run with 15+ Claude Code sessions in parallel. Each skill fixes one problem that kept happening there.

| Skill | What it fixes |
|---|---|
| [one-pass](https://github.com/RabbitDesigns22/one-pass) | get it right the first time; stop paying tokens for rework |
| [hora-exacta](https://github.com/RabbitDesigns22/hora-exacta) | real date and time in every message, so nothing lands on the wrong day |
| [hands-on](https://github.com/RabbitDesigns22/hands-on) | the agent does what it can and only asks you for codes, keys and payments |
| [one-answer](https://github.com/RabbitDesigns22/one-answer) | one thought-through answer instead of plan, fix, new plan |
| [never-twice](https://github.com/RabbitDesigns22/never-twice) | a shared error log so no session repeats a known mistake |
| [report-now](https://github.com/RabbitDesigns22/report-now) | status checked live this minute, stamped with the time |
| [sort-me-out](https://github.com/RabbitDesigns22/sort-me-out) | one ordered list of what is urgent, waiting and forgotten |
| [in-the-loop](https://github.com/RabbitDesigns22/in-the-loop) | a live board so parallel sessions know what the others changed |
| [study-first](https://github.com/RabbitDesigns22/study-first) | reads everything in full and answers point by point, no invented details |
| [session-watchdog](https://github.com/RabbitDesigns22/session-watchdog) | wakes the sessions that got stuck mid-task, leaves the rest alone |
| [skill-harvest](https://github.com/RabbitDesigns22/skill-harvest) | reads your sessions and finds the skills you are missing |
| [small-budget-ads](https://github.com/RabbitDesigns22/small-budget-ads) | Meta Ads rules for 1-5 USD a day ad sets |
| [whatsapp-closer](https://github.com/RabbitDesigns22/whatsapp-closer) | evidence-ranked rules for a WhatsApp sales assistant that closes |
| [whatsapp-number-onboarding](https://github.com/RabbitDesigns22/whatsapp-number-onboarding) | connect a number to the WhatsApp Cloud API in the safe order |
| [proposal-pdf](https://github.com/RabbitDesigns22/proposal-pdf) | short PDF proposals with every price checked against its source |
| [published-vs-planned](https://github.com/RabbitDesigns22/published-vs-planned) | says "published" only for what it saw live on the public page, Facebook and Instagram checked apart |
| [source-every-fact](https://github.com/RabbitDesigns22/source-every-fact) | every price, phone and name on a post traced to its source, nothing added |
| [only-what-was-asked](https://github.com/RabbitDesigns22/only-what-was-asked) | "pause only Google Ads" pauses only Google Ads, and proves the rest did not move |
| [model-per-chat](https://github.com/RabbitDesigns22/model-per-chat) | the right model for each chat: top model where mistakes cost money, cheap or none where it only runs often |

If one of them saved you a redo, a star helps other people find it.

## License

MIT. Made by [Rabbit Designs](https://github.com/RabbitDesigns22).
