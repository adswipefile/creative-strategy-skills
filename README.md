# Creative strategy skills for Meta ads

Agent skills for creative strategists who make Facebook and Instagram ads:
competitor research, personas, hooks and angles, ad concepts and creative audits, each backed by real ads from the
[Ad Swipe File ad library](https://adswipefile.com/?utm_source=github&utm_medium=referral&utm_campaign=creative-strategy-skills).

Ask Claude, ChatGPT, Codex or Cursor for a creative strategy and the agent
searches the library, reads the ads and writes from them, with a link to every
ad it cites.

## Install

With [skills.sh](https://skills.sh), in any agent it supports (Claude Code,
Codex, Cursor and others):

```bash
npx skills add adswipefile/creative-strategy-skills
```

Or copy a folder from `skills/` into your agent's skills directory
(`~/.claude/skills/` for Claude Code).

## Connect the ad library

The skills read the Ad Swipe File ad library through its MCP server, so connect
it once:

```bash
claude mcp add --transport http adswipefile https://adswipefile.com/api/mcp
```

On claude.ai or ChatGPT, add `https://adswipefile.com/api/mcp` as a custom
connector. Other clients: [MCP setup](https://adswipefile.com/docs/mcp?utm_source=github&utm_medium=referral&utm_campaign=creative-strategy-skills).
Connecting opens a browser sign-in to your Ad Swipe File account
([plans](https://adswipefile.com/pricing?utm_source=github&utm_medium=referral&utm_campaign=creative-strategy-skills)).

Prefer one install for the skills and the connection? The
[Ad Swipe File plugin](https://github.com/adswipefile/adswipefile-plugin) ships
both for Claude Code, ChatGPT, Codex, Cursor and Grok.

## The skills

Start with `creative-strategy`: it routes research, ideas, making, review and
learning to the right skill.

| Skill | What it does |
| --- | --- |
| [`audit-ad-creative`](skills/audit-ad-creative/SKILL.md) | Audit one ad creative, your own or a reference from the Ad Swipe File library, for why it lands or doesn't, judged from a stranger scrolling at speed, and return a short ranked feedback note where every problem ends in a fix. |
| [`competitor-ads`](skills/competitor-ads/SKILL.md) | Show what ads a brand or competitor is running in the Ad Swipe File ad library, and sum up the formats, hooks, angles and offers it repeats, with a link to every ad cited. |
| [`creative-strategy`](skills/creative-strategy/SKILL.md) | Start here for creative strategy on Meta ads with Ad Swipe File as the evidence. Routes research, ideation, making, review and learning to the right skill, from mapping competitors to concepts, scripts and audits. |
| [`find-winning-ads`](skills/find-winning-ads/SKILL.md) | Find winning Facebook and Instagram ads in the Ad Swipe File ad library by niche, format, brand or keyword, and present them with links. |
| [`generate-ad-concepts`](skills/generate-ad-concepts/SKILL.md) | Generate ad concepts by walking the map from anchor, persona, awareness stage and trigger moment to angle, offer statement, mechanic, format and hook, one concept or a full-funnel batch, with reference ads from the Ad Swipe File ad library for each step. |
| [`get-started`](skills/get-started/SKILL.md) | Set up Ad Swipe File after installation, check its connection when asked, and help the user ask a first question about winning ads, competitor ads or hooks. |
| [`map-competitors`](skills/map-competitors/SKILL.md) | List a brand's direct competitors, indirect competitors and the brands whose ads are worth admiring, each with why it is on the list, its Facebook page and whether the Ad Swipe File ad library holds its ads. |
| [`map-personas`](skills/map-personas/SKILL.md) | Find every persona in a product's customer reviews (who they are, the words they call themselves, variations, overlaps and filmable trigger moments), then pull reference ads for each persona from the Ad Swipe File ad library. |
| [`pick-creative-mechanic`](skills/pick-creative-mechanic/SKILL.md) | Choose, name or rebuild the creative mechanic of an ad (the move that makes the viewer reach the point themselves, between angle and format) from a fixed vocabulary matched to awareness stage, with built examples from the Ad Swipe File ad library. |
| [`record-creative-learning`](skills/record-creative-learning/SKILL.md) | Close the creative loop: turn your own ad results (an ads manager export, a report, numbers you paste) or an audit into a scoped learning (the why, not the what), write it back into the next concepts, and find Ad Swipe File reference ads for what to make next. |
| [`review-saved-ads`](skills/review-saved-ads/SKILL.md) | List the ads the user saved on adswipefile.com and find what they have in common: formats, niches, hooks, angles and offers. |
| [`teach-ad-breakdown`](skills/teach-ad-breakdown/SKILL.md) | Coach a daily direct-response rep: take one ad from the Ad Swipe File library and what the learner noticed, name the principle behind each observation, show what they missed and where the ad breaks its format's pattern, and end on one takeaway saved to their board. |
| [`track-competitor-ads`](skills/track-competitor-ads/SKILL.md) | Follow a brand's competitors on Ad Swipe File so their new Meta ads show up, and read what each one keeps running: brand patterns, longest-running ads, hooks, formats and offers. |
| [`weekly-competitor-review`](skills/weekly-competitor-review/SKILL.md) | Write a short weekly review of the new Meta ads the user's followed brands launched on Ad Swipe File, what changed against each brand's usual patterns, and three ideas to try, with a link to every ad. |
| [`write-hooks-from-ads`](skills/write-hooks-from-ads/SKILL.md) | Read winning ads in the Ad Swipe File ad library, name the hook and angle each one uses, and write original hooks, headlines or ad copy for the user's product in those patterns. |

## What you can ask

- "Build a creative strategy for my skincare brand."
- "Who are my competitors, and what ads are they running?"
- "Which hooks and formats are rising in my niche?"
- "Give me five ad concepts for cold traffic, with reference ads."
- "Write hooks for my product from ads that kept running in my niche."
- "Audit this ad and tell me what to fix."

## About this repo

The skills are plain Markdown instructions: no scripts, hooks or executables.
This repo is generated from the Ad Swipe File source and overwritten on every
release, so open an issue rather than a pull request for a change to a skill.

MIT licensed. Made by [Ad Swipe File](https://adswipefile.com/?utm_source=github&utm_medium=referral&utm_campaign=creative-strategy-skills).
