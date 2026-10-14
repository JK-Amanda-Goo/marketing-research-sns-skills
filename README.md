# Marketing Research: SNS Skills (Claude Code)

Four small skills that research what works on social media, and who you are up against, for **your** product, then hand back a compact Google Sheet you can act on the same day.

| Skill | Researches |
|---|---|
| `marketing-research-instagram-vid` | Instagram Reels: hooks and formats |
| `marketing-research-instagram-carousel` | Instagram carousels: covers, slide structure, caption CTAs |
| `marketing-research-tiktok-vid` | TikTok videos: hooks and formats |
| `marketing-research-competitors` | Competitors and substitutes: positioning, pricing, channels, customer voice, white space |

They are built for a fresh start: no prior brand context needed. Each one asks a few questions first, including the one that shapes everything: **is going viral or building credibility in your industry more important right now?** (The competitors skill asks which decision the research should support instead.)

## What you get

One Google Sheet. The three social skills share the same 3 tabs:

1. **Setup & Method**: goal, your context, priority, how the research was done, sample, evidence rule, limits.
2. **Best Practices**: up to 10 patterns, each marked Best practice / Hypothesis / Do not copy, with a fill-in-the-blank template for your own version.
3. **Log Highlights**: 15 to 20 example posts with basic numbers and a clickable link to each original.

The **competitors** skill adds a 4th tab, **Customer Voice** (sourced quotes with links), and its Best Practices tab holds Copy / Avoid / White-space moves with a next action each.

Evidence rule: a pattern is a "Best practice" only if it appears in 3 or more posts from 2 or more accounts. Anything thinner is labelled a hypothesis.

## Install

```bash
git clone https://github.com/JK-Amanda-Goo/marketing-research-sns-skills.git ~/marketing-research-sns-skills
for s in marketing-research-instagram-vid marketing-research-instagram-carousel marketing-research-tiktok-vid marketing-research-competitors; do
  ln -s ~/marketing-research-sns-skills/skills/$s ~/.claude/skills/$s
done
```

## Use

Ask Claude Code, for example:

- "Research Instagram Reels for my skincare brand."
- "Do carousel research for a B2B newsletter."
- "Find TikTok hooks that work for a coffee subscription."
- "Research competitors for my budgeting app before launch."

Needs: Claude Code with the Chrome browser tool (to read public pages), and a Google Drive connector if you want a native Google Sheet (otherwise you get an `.xlsx`).

## Limits, stated up front

- Public pages only; links are recorded, nothing is downloaded.
- Saves, shares and reach are mostly not public, so likes and comments are partial signals.
- Search results favour hits, so examples lean toward what already worked.
- If a site blocks automated access, the skill stops and continues by hand instead of working around it.
- Samples are small (about 25 to 40 posts). Read results as strong hints, not statistics.

## License

MIT
