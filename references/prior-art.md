# Prior art: anti-slop design skills

Researched 28 September 2026 from each repo's skill and rule files. Everything below is paraphrased. Star counts come from the GitHub API on that date. Credit these projects in the README if any idea is adopted.

| Project | Licence | Stars | How it works |
| --- | --- | --- | --- |
| anthropics/skills, frontend-design | Apache-2.0 | ~179k | Instructions |
| pbakaus/impeccable | Apache-2.0 | ~72k | Instructions plus code detector rules |
| Leonxlnx/taste-skill | MIT | ~91k (unusually high, unverified) | Instructions, pre-flight checklist, three style dials |
| Nutlope/hallmark | MIT | ~29k | 58-gate self-review checklist |
| miqdadbadjuber/anti-slop (fork: fajarhide) | MIT | ~3.9k | 38 rules, reason required for each default |
| Trystan-SA/claude-design-system-prompt | MIT | ~2k | System prompt plus review skill |
| codeswithroh/tastemaker | MIT | ~420 | Checklist, self-critique, Python detectors, style lock |
| Gesso-Build/skills (anti-slop) | MIT | ~90 | Static detector with auto-fix tiers |
| Laith0003/ux-skill | MIT | ~76 | Regex rules (README only read) |
| Ferousco-dev/anti-slop-design | MIT | ~14 | Instructions |
| claudiusararu/unslop-ui-skill | MIT | 2 | Catalogue of about 150 tells |

## Banned by three or more projects

- Purple, violet or blue decorative gradients, including gradient text.
- Grids of identical cards with an icon on top, and default card kits.
- Nested cards, and cards with a coloured stripe on one edge.
- Eyebrow labels above headings, tracked-out capitals, and 01/02/03 markers.
- Overused default fonts: Inter, Geist, Roboto, Arial, Space Grotesk.
- Reflexive cream or beige palettes.
- Glassmorphism, glows, aurora blobs and halos.
- Fade-up animation on every section, blanket hover-scale, bounce or overshoot easing.
- Emoji and sparkle icons.
- Invented statistics, testimonials and trust claims.
- Buzzwords ("seamless", "revolutionary", "supercharge") and generic calls to action ("Get Started", "Learn More").
- Heavy em-dash use.
- The stock template: hero, three features, call to action, standard nav and four-column footer.
- Monospace type used as decoration.

## Distinctive bans from single projects

- Anthropic: a near-black page with one acid-green or vermilion accent; arrows appended to buttons; strings joined with middle dots; the "broadsheet" look of hairline rules, zero radius and dense columns.
- Impeccable: pulsing status dots; letter-spacing tighter than -0.04em; display type larger than 6rem; body text under 16px.
- taste-skill: a named "premium" palette of cream, brass, oxblood and espresso; pure black or white; each layout type used once per page; fake product screenshots built from boxes; city, time and weather strips; "scroll to explore" cues; placeholder brand names like Acme.
- Hallmark: italic headings of any kind; curly quotes required; no two-line buttons; no redrawn browser or phone frames.
- anti-slop: every em dash; copying Linear, Vercel or Stripe; a written reason for each major design choice.
- tastemaker: layouts must differ from previous builds; banned sentence templates such as "where X meets Y" and "reimagined"; no letter-in-a-box logo.
- Gesso: "it's not X, it's Y" phrasing; oversized card radius clamped; ghost-card shadows.
- Ferousco: dark mode nobody asked for; chart axes not starting at zero.

## Where this skill differs

These projects mostly target startup and software landing pages, so several of them ban conventional structure such as a standard nav, a four-column footer, square hairline layouts and arrows on buttons. This skill targets established small businesses and organisations, where those conventions are correct because visitors expect them. It learns from real sites in each sector instead of banning the ordinary.

Conflicts to resolve if adopting ideas: Anthropic discourages the square, hairline "broadsheet" look that this skill's baseline uses. Hallmark requires em dashes in place of double hyphens, while anti-slop bans them entirely.
