# easy-for-them

**When a person has to do something, make it almost effortless.**

`easy-for-them` is an agent skill for Claude Code (and any agent that reads `SKILL.md` skills). Agents love to answer with "go to Settings, then Billing, then Accounts, then...". Busy people, and especially your clients on a phone, get lost and give up. `easy-for-them` makes the agent remove every step it can, give direct links that land on the exact screen, write one action per line in plain words, and hand you a message ready to forward to your client as-is.

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

## License

MIT. Made by [Rabbit Designs](https://github.com/RabbitDesigns22).
