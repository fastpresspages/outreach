# 12 open-source ideas, ranked

**Status:** candidate list, not a roadmap. Nothing here is promised until it ships.

Ranking is by **usefulness × distribution ÷ effort**, not by how fun it is to build. Every idea must be free to use, cheap to host, and honest about what it does.

| # | Idea | Effort | Distribution | Verdict |
| --- | --- | --- | --- | --- |
| 1 | **FastPress Start** — zero-build launch-page template | 3 days | High: forkable, visual, solves a real first step | **Shipped 24 Oct 2026** |
| 2 | **Public teardown library** — dated before/after audits | 1 day each | High: specific, shareable, SEO | Start with 3 |
| 3 | **LaunchGrade Action on Marketplace** | 1 day | High: GitHub-native, recurring use | Do now |
| 4 | **Agent-ready report** — how AI crawlers see your page | 3 days | Medium-high: timely, technical | After template |
| 5 | **Free audit clinic** — monthly live teardown | 1 day/month | Medium: trust, leads | Schedule |
| 6 | **Community check registry** — contributed checks + fixtures | 1 week | Medium: contributors, credibility | After 50 users |
| 7 | **Ship Log** — weekly public changelog + lesson | 2 hours/week | Medium: habit, retention | Start small |
| 8 | **MCP directory push** — list the server where agents look | 1 day | Medium: compounding discovery | Do now |
| 9 | **Awesome Launch Pages** — curated list with a pass bar | 2 days + upkeep | Medium: links, but risk of link farm | Later |
| 10 | **Launch copy checklist** — one-page pre-launch guide | 1 day | Medium: SEO, email attachment | Later |
| 11 | **Local-business audit** — niche paid offer | 1 week | Low-medium: sales-heavy | Test one |
| 12 | **Sponsor kit** — transparent tiers for the tools | 1 day | Low now: no audience yet | After traction |

---

## 1. FastPress Start — zero-build launch template

**Problem:** people launching a first page do not need a framework; they need a page that loads fast, has a clear CTA, captures email, and does not look generic.

**MVP:** one `index.html`, one `styles.css`, one `app.js`. Sections: hero, proof, one CTA, FAQ, contact form, privacy/terms, `llms.txt`, `robots.txt`, `sitemap.xml`, OG image, JSON-LD. A README that says exactly what to edit in 15 minutes.

**Why it fits:** it is the same stack as YouLauncher and the hire page. It can be audited by LaunchGrade and shipped with a real A+ report. It gives people a reason to try the CLI before they have a page.

**Distribution:** "Fork this, change five lines, ship today" post; before/after screenshots; submit to template directories; use it for every future FastPress page.

**Do not:** add a build step, a paid font, a tracking script or a fake testimonial section.

## 2. Public teardown library

**Problem:** "best practices" is abstract. A dated teardown of a real public page is concrete.

**MVP:** one Markdown/HTML report per page: what it does well, the three fixes with the highest impact, the LaunchGrade score before/after if the owner ships changes. Only public pages; no private analytics; no snark.

**Why it fits:** content that demonstrates the product without a sales pitch. Each teardown is a shareable artifact and a permanent search result.

**Distribution:** X/LinkedIn carousel, Indie Hackers post, Hacker News only if the lesson is genuinely technical, newsletter pitch.

**Do not:** shame a solo founder, publish a "before" without context, or claim the owner endorsed it.

## 3. LaunchGrade Action on Marketplace

**Problem:** the action exists, but people do not discover it from a README alone.

**MVP:** publish the existing composite action to GitHub Marketplace, add a `uses: fastpresspages/launchgrade@v0.1.0` snippet, a sample workflow and a screenshot of the PR comment/output.

**Why it fits:** zero new runtime, direct distribution to people already shipping on GitHub.

**Do not:** make it fail every PR by default. Start with `fail-under: 0`, let teams opt into a gate.

## 4. Agent-ready report

**Problem:** "AI SEO" is mostly noise. Teams need a concrete answer to: can agents fetch, parse and trust this page?

**MVP:** a LaunchGrade mode that reports `llms.txt`, `AGENTS.md`, markdown negotiation, robots rules for GPTBot/ClaudeBot/PerplexityBot, MCP/OpenAPI discovery, semantic HTML and no-JS content. Output one page with evidence.

**Why it fits:** LaunchGrade already has the checks and the category. The standalone report is a clearer story than a number.

**Do not:** promise rankings in ChatGPT or claim an "AI visibility score" that cannot be measured.

## 5. Free audit clinic

**Problem:** a form is passive. A monthly live teardown creates a reason to show up and a reason to trust the method.

**MVP:** 45 minutes, two volunteer pages, LaunchGrade run live, three fixes each, recording and written summary. Free, no pitch beyond "email me if you want help."

**Why it fits:** it turns the audit into a community event and produces clips, posts and case studies with consent.

**Do not:** ambush a founder, critique a page without permission, or turn the Q&A into a timeshare pitch.

## 6. Community check registry

**Problem:** one maintainer's checklist is limited. Contributors see checks the maintainer misses.

**MVP:** a documented check contract, one fixture per check, a registry file, and a review rule: a check must be specific, testable and free of vendor lock-in. Start with five contributed checks, not fifty.

**Why it fits:** it gives contributors a small, useful first PR and makes the tool more credible.

**Do not:** accept checks that require a paid API, a specific CMS or a subjective "looks good" judgment.

## 7. Ship Log

**Problem:** people forget a project exists between launches.

**MVP:** one short post per week: what shipped, one number with a source, one lesson, one ask. Published in GitHub Discussions and cross-posted. No "10x" language.

**Why it fits:** a habit beats a launch spike. It also creates a public archive of progress.

**Do not:** write a post when nothing shipped. "We are still working" is not a ship log.

## 8. MCP directory push

**Problem:** the MCP server is only discoverable if someone reads the README.

**MVP:** submit to `punkpeye/awesome-mcp-servers`, the official MCP servers list if eligible, `mcp.so` and `smithery.ai`; add a copy-paste config and a 30-second demo.

**Why it fits:** agent users are a small but high-intent audience, and the server is already zero-dependency.

**Do not:** spam every directory with the same blurb. Read the submission rules; skip paid placements if there is no budget.

## 9. Awesome Launch Pages

**Problem:** there is no trusted, small list of launch pages that do the fundamentals well.

**MVP:** 20 pages, each with a one-line reason and a LaunchGrade score. Submission via issue. A page must score A- or higher and be publicly inspectable.

**Why it fits:** curation is cheap and linkable. It also creates a quality bar for the tool.

**Do not:** let it become a link farm. Remove dead pages, disclose any relationship, and never charge for a spot.

## 10. Launch copy checklist

**Problem:** the audit tells you what is missing, but not how to write the fix.

**MVP:** one page: headline, subhead, proof, CTA, objections, privacy, FAQ. Before/after examples from real pages. Downloadable as Markdown.

**Why it fits:** it pairs naturally with the CLI and can be emailed after an audit.

**Do not:** sell it as a "conversion guarantee" or fill it with generic advice.

## 11. Local-business audit

**Problem:** local businesses have launch pages too, and often no technical help.

**MVP:** one niche (e.g. independent cafés or studios), a one-page audit, a fixed price for three fixes, and a before/after. Test with two businesses, not twenty.

**Why it fits:** it can fund the free tools. It is also a much harder sales motion; be honest about that.

**Do not:** cold-call with a fake "I noticed your website is losing customers" line. Lead with a real, specific observation.

## 12. Sponsor kit

**Problem:** free tools still cost time and hosting.

**MVP:** a simple page: what is free, what sponsorship pays for, three tiers, no fake "500k impressions". Start with one sponsor and a named deliverable.

**Why it fits:** it is a clean alternative to ads and paid placements.

**Do not:** sell a "featured check" that changes a score. The audit must stay independent.

---

## What to build next

**FastPress Start is live:** [fastpresspages.github.io/fastpress-start](https://fastpresspages.github.io/fastpress-start/), with a dated A+ 100/100 audit.

**RepoGrade (project 7) is live instead of a new template:** [fastpresspages/repograde](https://github.com/fastpresspages/repograde) shipped on 24 Oct 2026 — the repo-side twin of LaunchGrade (33 checks: docs, community, engineering, discoverability, release hygiene, agent-readiness). Dogfood: **A+ 99/100** on its own repo; LaunchGrade-audited site at **A+ 100/100**. Both projects feed each other and both share the same zero-dep philosophy; the "Agent-ready report" idea above is covered by RepoGrade's agent-ready category (AGENTS.md / skills / MCP / llms.txt checks), so that slot is closed.

If only one thing gets distributed this month: **three public teardowns**. They prove the method better than any thread.
