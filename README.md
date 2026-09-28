# human-site-style

A Claude Code skill for building small-business websites that don't look AI-generated.

I built this while [Sophenor](https://github.com/Sophenor) and I were working on our first web-design project, making a new website for a Somerset tourist farm. We asked Claude for a first draft, and what came back was generic, completely lacking in personality, with design features that made it look heavily AI-generated (zoom-on-scroll effects, pill buttons etc.) So, instead of relying on Claude's averaged design sense, I thought it was a good idea to write a skill that learnt from good-looking websites whose design actually suited the kind of business we were building for.

## What it does

Ask Claude for a website and the skill loads on its own. Claude then:

1. Asks for a brief first: what the business does, the one action that matters (an enquiry, a booking), what real photos and content exist, and what brand it already has.
2. Picks a style for the type of business and builds from a baseline taken from real sites.
3. Checks the page against a set of hard rules and an avoid list, and fixes what fails before it says it's done.

Hard rules, which no style overrides:

- no pill-shaped buttons
- no cream page background (cream sections are fine)
- no gradients
- no em dashes
- no invented figures, testimonials, prices or opening times
- no AI-sounding copy (see `references/writing.md`)

## Styles

| Style | For | Examples it learned from |
| --- | --- | --- |
| Baseline | any business | consultancies such as Kalypso, Baringa, Odgers |
| Professional services | consultancies, advisers, firms | the same |
| Heritage attraction | stately homes, castles, gardens, museums | Chatsworth, Blenheim, Hever, Leeds Castle |
| Family attraction | farms, safari parks, activity centres | Longleat, Woburn, Diggerland |

More styles will be added as they come up.

## How it differs from other so-called anti-slop skills

Most of the existing ones (listed below) are aimed at startup and SaaS landing pages, so they ban a lot of conventional structure: a standard nav bar, a four-column footer, square layouts. For a farm shop or a local firm that structure is right, because it's what visitors expect. So instead of only banning things, this skill copies what real businesses in each sector do, from fonts and colours read off their live pages.

## Install

```bash
git clone https://github.com/Seraphine-ops/human-site-style.git ~/.claude/skills/human-site-style
```

Start a new Claude Code session afterwards. To update, `git pull` in that folder.

## Files

```
SKILL.md                    the instructions Claude follows
references/site-notes.md    what each reference site does (fonts, colours, buttons, layout)
references/writing.md       words, phrases and patterns to avoid in copy
references/prior-art.md     other anti-slop skills and what they ban
SECURITY.md                 what the skill can and can't do, and how to report problems
```

## Credits

The rules were written for this repo, but a lot of the thinking came from reading these projects. 

- [anthropics/skills](https://github.com/anthropics/skills) frontend-design (Apache-2.0)
- [pbakaus/impeccable](https://github.com/pbakaus/impeccable) (Apache-2.0)
- [Nutlope/hallmark](https://github.com/Nutlope/hallmark) (MIT)
- [miqdadbadjuber/anti-slop](https://github.com/miqdadbadjuber/anti-slop) (MIT)
- [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) (MIT)
- [claudiusararu/unslop-ui-skill](https://github.com/claudiusararu/unslop-ui-skill) (MIT)

Writing rules credits are in `references/writing.md`.

## Licence

MIT
