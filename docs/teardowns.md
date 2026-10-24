# Public teardowns — 24 Oct 2026

Real launch pages from fresh Show HN posts, graded with [LaunchGrade](https://github.com/fastpresspages/launchgrade) v0.3.0. All numbers come from the tool's own output; full reports are committed under `teardowns/<slug>/` and served live on the [field scans page](https://fastpresspages.github.io/launchgrade/teardowns/).

## The scans

| Page | HN points | Grade | Pass / warn / fail | Weakest category | Top fix |
|---|---|---|---|---|---|
| [Permit](https://permit.petercai.com/) ([HN](https://news.ycombinator.com/item?id=50170593) 936 pts) | 936 | **B- 73** | 31 / 12 / 3 | Trust 38 | No privacy policy, no email capture |
| [Swurf](https://swurf.org/) ([HN](https://news.ycombinator.com/item?id=50205320) 72 pts) | 72 | **C+ 65** | 22 / 18 / 5 | Trust 31 | Privacy policy; buttons without accessible names |
| [Corgi](https://corgi.computer/) ([HN](https://news.ycombinator.com/item?id=50214373) 102 pts) | 102 | **D+ 53** | 20 / 19 / 7 | Conversion 37, Trust 38 | No email capture, no CTA, 1.4 MB of HTML |
| [Impossible Machines](https://www.impossiblemachines.xyz/) ([HN](https://news.ycombinator.com/item?id=50202746) 76 pts) | 76 | **D+ 54** | 19 / 19 / 6 | Social 20 | No Open Graph card, no privacy policy, no seed capture |

Selection bias, stated openly: these are LaunchScore-unaware pages from one day of Show HN, chosen because they were public, popular and easy to verify. They are not the best or worst launches on the internet — they are a normal sample.

## The pattern (this is the story worth telling)

1. **Trust 38 on all four.** Not one fresh launch links a privacy policy. It is the single most common fail and takes an hour to fix.
2. **No email capture on any of them.** HN sends a spike that dies in ~48 hours. All four let it vanish with nothing left behind.
3. **Half missing OG cards.** 2 of 4 have no preview image — the link still travels to X/Discord/Slack but naked.
4. **None speak to agents.** No llms.txt, no agent-facing summary anywhere.
5. **The technical floor is high.** Technical 90–98 everywhere. Builders ship fast, secure pages; what's missing is the human layer (capture, trust, share).

## Public artifacts

- Field-scan index: https://fastpresspages.github.io/launchgrade/teardowns/
- Per-project reports: `teardowns/{corgi,swurf,permit,impossible-machines}/report.html` (also on the live site under the same path).

## Etiquette policy for this series

1. Public pages only; numbers come from running tool output, dated.
2. Lead with what the page does well before the fixes.
3. Never email the authors uninvited. The offer lives in public: take the fixes, or ping the [free audit form](https://fastpresspages.github.io/launchgrade/#audit).
4. Corrections and removals: issue or email, acted on within a day.
5. No private data: only what the page itself publishes plus optional public HN points.

## Next teardowns

- Re-scan in ~1 week: did any of the four fix the top items? (`--compare` against these baselines is built for exactly that.)
- New launches preferred (HN 0–48 h) so advice lands while it still matters.
