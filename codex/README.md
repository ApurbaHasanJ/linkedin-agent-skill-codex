# LinkedIn Agent Skills for Codex

This is a Codex adaptation of [Jakeschincariol/linkedin-agent-skill](https://github.com/Jakeschincariol/linkedin-agent-skill), which is the upstream Claude skill pack. The Codex edition preserves all eleven workflow names and their core purposes:

| Skill | What it does |
|---|---|
| `li-post` | Turn one idea into a post with three hooks and a copy-ready draft. |
| `li-comment` | Draft specific comments on posts the user supplies. |
| `li-reply` | Triage and draft replies to comments on the user's post. |
| `li-profile` | Score and rewrite profile sections from supplied profile text. |
| `li-plan` | Make a weekly content and engagement plan. |
| `li-human` | Clean text and run the included local heuristic checks. |
| `li-carousel` | Write a LinkedIn carousel, slide by slide. |
| `li-repurpose` | Extract standalone posts from long-form material. |
| `li-dm` | Draft a connection note and follow-up sequence. |
| `li-inbox` | Triage messages supplied by the user and draft selected replies. |
| `li-audit` | Analyze post metrics supplied by the user. |

## What “keep the commands” means in Codex

Codex packages these workflows as Agent Skills, not Claude Code slash commands. The names stay `li-post`, `li-comment`, and so on. Invoke a skill explicitly with `$li-post` in Codex CLI or the IDE extension, or select it from the Skills picker in the ChatGPT desktop app. Depending on the Codex surface, you can also describe the task and let its skill description trigger it. A third-party repository cannot register Claude-style `/li-*` commands in Codex by renaming text; slash commands are controlled by the Codex host.

## Install

For an individual workflow, use Codex's skill installer with a path from this repository, for example:

```text
$skill-installer https://github.com/OWNER/REPO/tree/main/codex/skills/li-post
```

Repeat for the other skill names. The upstream `skills/` directory remains intact for Claude Code. Codex-ready versions are under `codex/skills/`.

## Voice and local state

Put a voice profile at `~/.codex/linkedin/voice.md` for local Codex installs. The `li-post` folder includes `voice.template.md`. If the active ChatGPT/Codex surface cannot read that local file, paste the profile or three example posts into the conversation. Planning and log files are optional: skills should work from material supplied in the conversation when local files are unavailable.

## Boundaries

These skills draft and analyze; they do not log into LinkedIn, scrape its feed or inbox, publish posts, send DMs/comments, or schedule content. The `li-human` scores are local heuristics, not detector results or promises that text is undetectable. Scripts require Python 3 and have no third-party dependencies.

## License and credit

The upstream project and this adaptation are licensed under MIT. Keep the included copyright and permission notices when redistributing. The original project was created by Jake Schincariol. This repository is an independent adaptation and is not affiliated with or endorsed by the original author or OpenAI.
