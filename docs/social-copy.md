# Social copy

**Post only when the artifact exists.** Every link below should resolve. Every number should have a date and a source. If a line feels like a growth hack, delete it.

## X / Twitter thread

**1/**
I built a free CLI that grades a launch page in about 60 seconds.

53 checks. 7 categories. Zero dependencies.

No account. No paid API. No "book a demo".

`npx -p github:fastpresspages/launchgrade launchgrade your.site`

**2/**
The first page I scanned was my own.

It scored **B- 71/100**.

The conversion was fine. The trust signals were not: no privacy page, no Open Graph card, no `llms.txt`.

Not a great look for a page about trust.

**3/**
The 7 categories:

• Conversion 25%
• Trust 15%
• Technical 20%
• SEO 15%
• Social 10%
• Accessibility 5%
• AI-agent readiness 10%

Every check has an ID, a weight and a fix you can act on.

**4/**
The report is not a dashboard you have to interpret.

It gives you a letter grade, category scores, and the fixes sorted by impact.

Terminal, Markdown, JSON, a standalone HTML report and an SVG badge.

**5/**
I rebuilt the page.

Same offer. Real proof instead of invented testimonials. A privacy page. Open Graph. `llms.txt`. A two-field form.

The next scan: **A+ 100/100**, with one deliberate warning because the page has no analytics.

Before: [link]
After: [link]

**6/**
It also runs in CI:

```yaml
- uses: fastpresspages/launchgrade@v0.1.0
  with:
    url: https://your.site
    fail-under: 80
```

And it ships an MCP server, so agents can run the same audit:

```json
{"mcpServers":{"launchgrade":{"command":"npx","args":["-y","-p","github:fastpresspages/launchgrade","launchgrade-mcp"]}}}
```

**7/**
The whole thing is Apache-2.0 and zero-dependency.

No telemetry. No account. No upsell in the CLI.

If a check is wrong, the fixture is in the repo and the issue template is open.

**8/**
Want a free human audit of your launch page?

Send the URL: [audit link]

I read every one. If the report is useful, use it. If you want help with the fixes, that is a separate conversation.

No fake urgency. No countdown.

## Show HN

**Title:** `Show HN: LaunchGrade – grade any launch page in 60 seconds (zero deps)`

**Body:**

> I built a CLI that audits a public launch page across conversion, trust, technical, SEO, social, accessibility and AI-agent readiness. It is free, Apache-2.0 and has zero runtime dependencies.
>
> The first scan of my own page scored B- 71/100. The fixes became the roadmap; the rebuilt page scored A+ 100/100 with one deliberate warning (no analytics). Both reports are public.
>
> What it does: fetches the page (and robots.txt, sitemap.xml, llms.txt, security.txt), runs 53 checks, weights them, and prints a grade plus the highest-impact fixes. It can also write HTML/Markdown/JSON reports, an SVG badge and a fix plan.
>
> What it does not do: measure real conversion, replace a security review, or guarantee rankings. It is a heuristic, and the checks are public so you can disagree with them.
>
> Install: `npx -p github:fastpresspages/launchgrade launchgrade your.site`
>
> Source and sample reports: https://github.com/fastpresspages/launchgrade
>
> I would especially value feedback on checks that are wrong, missing or too subjective. The check contract and fixtures are in the repo.

**Do not:** ask for upvotes, post the same text in five communities, or argue with criticism in the thread.

## Product Hunt

**Tagline:** `Grade your launch page before the internet does.`

**Description:**

> LaunchGrade is a free, zero-dependency CLI that scans a public launch page across 53 checks in 7 categories: conversion, trust, technical, SEO, social, accessibility and AI-agent readiness.
>
> Run one command. Get a letter grade, category scores and the fixes that matter most. Export a terminal summary, Markdown, JSON, a standalone HTML report or an SVG badge. Add it to GitHub Actions or call it from an MCP client.
>
> No account, no telemetry, no paid API. Apache-2.0. The checks and sample reports are public, including the B- 71 scan that started it.

**First comment:**

> Maker here. I built this after auditing my own launch page and finding the embarrassing stuff first: no Open Graph image, no privacy page, no `llms.txt`. The before/after reports are linked from the site.
>
> Happy to answer questions about the scoring, the checks, or why "AI-agent readiness" is mostly about being readable without JavaScript. If a check is wrong, tell me and I will fix it in public.

**Do not:** offer a discount for upvotes, run a giveaway, or ask friends to comment.

## Reddit

### r/SideProject

**Title:** `I built a free CLI that grades launch pages. My own page scored B- 71.`

> I kept seeing launch pages with a clear offer and no trust signals. So I built a small open-source checker.
>
> It runs 53 checks across conversion, trust, technical, SEO, social, accessibility and agent readiness. It gives a grade and the top fixes, not a dashboard.
>
> The first page I scanned was mine: B- 71/100. No privacy page, no OG image, no llms.txt. I fixed it and published both reports.
>
> Free, zero deps, no signup: [link]
>
> Feedback welcome, especially "this check is wrong" feedback.

### r/webdev

**Title:** `Zero-dependency Node CLI that audits a page's technical/SEO/a11y basics`

> I built this because I wanted one command that checks the boring stuff before a launch: status, compression, canonical, meta description, one H1, alt text, form labels, robots, sitemap, OG tags.
>
> It also checks agent-readability: llms.txt, markdown negotiation, AI crawler rules, semantic HTML.
>
> 53 checks, 7 categories, no runtime dependencies. Apache-2.0. Source and fixtures: [link]
>
> I am more interested in missing/wrong checks than in stars.

### r/SEO

**Title:** `A free technical SEO + launch-readiness checklist you can run locally`

> Not a ranking tool. It is a pre-launch sanity check: title/description length, one H1, canonical, sitemap, robots, schema, alt text, OG/Twitter cards, plus agent-readability files.
>
> It outputs a grade and the highest-impact fixes. The checks and weights are public, so you can argue with them.
>
> [link] — no signup, no email gate.

**Rules:** read each subreddit's self-promotion rules first. If a subreddit requires participation before posting, participate for a week. Do not cross-post the same title.

## LinkedIn

> I rebuilt my own launch page and removed every number I could not source.
>
> The first audit scored it **B- 71/100**: clear offer, weak trust. No privacy page. No Open Graph card. No `llms.txt`.
>
> The fixes were not glamorous. Add the pages. Write the meta tags. Cut the form to two fields. Publish the before and after.
>
> The next scan: **A+ 100/100**, with one deliberate warning because the page has no analytics.
>
> I turned the checklist into a free, zero-dependency CLI: 53 checks across conversion, trust, technical, SEO, social, accessibility and AI-agent readiness. Apache-2.0. No account, no telemetry.
>
> The lesson is not "get an A+". It is that trust is made of small, checkable things. If you cannot show the source, do not put it on the page.
>
> Free audit: [link]

**Do not:** add "thoughts?" as a fake engagement question. Ask a real question if you have one.

## Indie Hackers

**Title:** `I deleted the fake case studies from my launch page. Then I audited it.`

> My launch page had the usual stuff: a big claim, a few testimonials, numbers without a source. I could not defend any of it.
>
> So I removed it and rebuilt the page around things I could link: public code, a passing test suite, dated before/after reports.
>
> Then I ran my own audit tool on it. B- 71/100. The trust signals were the problem.
>
> After the fixes: A+ 100/100, one intentional warning (no analytics). Both reports are public.
>
> I am not sharing this because the score is impressive. I am sharing it because removing the fake proof made the page easier to write and easier to defend.
>
> If you are pre-launch: what is one number on your page you cannot source?

## dev.to / Hashnode

**Title:** `53 checks, zero dependencies: how LaunchGrade audits a launch page`

Outline:

1. Why a heuristic, not a lighthouse clone.
2. The 7 categories and the weights.
3. How a check is defined (id, category, weight, `run`, pass/warn/fail/info).
4. Fetching the page and the extra files (`robots.txt`, `sitemap.xml`, `llms.txt`, `security.txt`).
5. Scoring: pass = 1, warn = 0.5, fail = 0; category normalization; impact sorting.
6. Report formats and the GitHub Action.
7. What the tool cannot know.
8. How to add a check with a fixture.

End with the repo link and a specific invitation: "If you know a check that is missing, open an issue with a fixture."

## Posting checklist

- [ ] The link works in a private window.
- [ ] The claim has a date and a source.
- [ ] The post gives something away before asking for anything.
- [ ] The community's rules allow this kind of post.
- [ ] I will reply to comments for at least two hours.
- [ ] I will not argue with criticism; I will ask what would make it useful.
- [ ] No upvote request, no engagement pod, no fake account.
