---
name: fastpress-goals
description: Run an honest weekly or 90-day review for FastPress Labs. Use when the user asks for a goal check-in, weekly review, outreach plan, launch retrospective, or "what should I do next" for the FastPress Labs community. Reads GOALS.md and the outreach docs, updates only sourced numbers, and picks one smallest useful action.
license: Apache-2.0
metadata:
  author: FastPress Labs
  version: "1.0.0"
---

# FastPress Goals

A small, honest operating system for [FastPress Labs](https://github.com/fastpresspages). It turns "how is it going?" into a dated scorecard and one next action.

## When to use

- A weekly review or a 90-day goal check.
- Planning the next launch, teardown, audit or outreach batch.
- Deciding whether to continue, narrow or stop a channel.
- A retrospective after a launch or a quiet month.

Do not use it to invent progress, generate fake testimonials or set vanity targets.

## Read first

1. [GOALS.md](https://github.com/fastpresspages/outreach/blob/main/GOALS.md) — targets, baselines, review questions.
2. [docs/launch-plan.md](https://github.com/fastpresspages/outreach/blob/main/docs/launch-plan.md) — the 30-day plan and kill criteria.
3. [docs/measurement.md](https://github.com/fastpresspages/outreach/blob/main/docs/measurement.md) — definitions and the scorecard.
4. [docs/ideas.md](https://github.com/fastpresspages/outreach/blob/main/docs/ideas.md) — the ranked candidate list.

## Workflow

### 1. Set the date and the period

Ask for the review date if it is not obvious. Use the actual date, not "this week". A review without a date is a mood.

### 2. Collect artifacts, not feelings

List what shipped since the last review, with a public URL or a commit. If there is no artifact, say "nothing shipped" and do not dress it up.

Examples:

- a merged PR or release;
- a published teardown or post;
- a completed audit with a report URL;
- a new check with a fixture;
- a page or template that is live.

### 3. Collect the numbers

For each number, record the value, the date and the source. Use only:

- GitHub Insights (traffic, clones, referrers);
- FormSubmit emails (`source`, `page`, `date`);
- the sent folder (personalized sends);
- the inbox (replies);
- your own notes (calls, audits, paid conversations).

If a number is unknown, write **unknown**. Do not estimate it and do not round it up.

### 4. Update the scorecard

Use the table in `docs/measurement.md`. Compute:

- reply rate = replies ÷ personalized sends;
- audit conversion = audits completed ÷ replies;
- paid conversion = paid pilots ÷ audits completed.

Compare to the previous four weeks, not to an unsourced "industry benchmark".

### 5. Answer the five review questions

1. What shipped? Link it.
2. Who replied? Aggregate unless the person opted in.
3. What did we learn? One sentence.
4. What is the next smallest useful thing? One action with a due date.
5. Did we publish anything we cannot source? If yes, fix it before the next send.

### 6. Choose one action

Pick the smallest action that could produce a real conversation this week:

- publish one teardown;
- send three personalized audit offers;
- fix one broken check;
- ship one template improvement;
- follow up once with an existing reply.

Do not pick five. One.

### 7. Flag stale claims

Scan the live pages and the last public post for numbers that are no longer true. If a claim is stale, mark it for correction today. Do not leave it up because it looks good.

## Output format

```markdown
## FastPress review — [date]

**Shipped**
- [artifact](url)

**Numbers**
| Metric | Value | Source |
| --- | --- | --- |
| ... | ... | ... |

**Rates**
- Reply rate: X% (n/n)
- Audit conversion: X% (n/n)
- Paid conversion: X% (n/n)

**Learned**
One sentence.

**Stale claims**
- None / [claim + fix]

**Next action**
One action, owner, due date.

**Decision**
Continue / narrow / stop [channel], because [source].
```

## Guardrails

- Never invent a metric, testimonial, customer, partnership or reply.
- Never change a baseline to make progress look better.
- Never add analytics to a FastPress page; use form fields and GitHub Insights.
- Never publish a person's name or email without permission.
- Never recommend mass email, bought lists, engagement pods or upvote requests.
- If a target is missed, say so. The miss is data.
- If there is no paid pilot by day 90, follow the decision in `GOALS.md`; do not fake demand.

## Install

```bash
npx skills add fastpresspages/outreach
```

Then ask your agent for a "FastPress weekly review".
