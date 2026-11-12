---
name: instagram-weekly-content-planner
description: Plans an Instagram account's week, researches which Reels work in the niche ranked by an outlier ratio (views divided by the account's median), and audits past posts. Use for "weekly plan", "what should I post", "viral research", "analyse my posts".
---

# Instagram Content Planner: Plan, Research, Audit

Works for any niche; set it once from the user's answers (see Plan → Input). Reply in the user's language. No Python tool needed: Claude does the arithmetic and shows the working. Nothing is posted, liked or followed: this skill writes and reads, the user publishes.

Three modes: **Plan** (weekly), **Research** (monthly), **Audit** (every 2–4 weeks). If the user doesn't say which, plan.

## Hook formula bank

Plan, research and audit share the same numbers, so you can track which formula works over weeks. Examples are written for a storytelling account (companies, founders, products); rewrite them for the user's niche. Fill `{{...}}` fields only with real, sourced information.

| # | Formula | Pattern | Example |
|---|---|---|---|
| 1 | Price of a mistake | {Amount} was the cost of {one mistake}. | "{{amount}}: the price of {{company}}'s single 'no'." |
| 2 | Reverse order | Stop {what everyone does}. {This one} did the opposite. | "Don't pay for ads. {{brand}} sold {{number}} with zero ads." |
| 3 | Nobody tells you | Nobody tells you {uncomfortable truth}. | "Nobody tells you how fast growth can sink a company." |
| 4 | Time collapse | It used to take {long}, now {short}. | "A car took 12 hours to build. Ford's assembly line cut it to 93 minutes." |
| 5 | The receipts | For {X} years they {did this}. Here are the real numbers. | |
| 6 | Inside leak | {Person} spent {N years} at {place}. Here's what nobody says out loud. | |
| 7 | Numbered + favourite | {N} {things}. Nobody uses number {k}. | |
| 8 | Before / after | {Old state}. {New state}. One thing changed. | |
| 9 | Call-out | {Specific group}, this is exactly what you're ignoring. | "Shop owners: this store made {{x}}× the revenue on the same rent." |
| 10 | Failure log | The first {N} {attempts} did nothing. On {N+1} this changed. | "Dyson built 5,126 prototypes. What changed on 5,127?" |
| 11 | Head to head | {A} or {B}? One wasn't even close. | |
| 12 | Deadline | {Thing} changes on {date}. | |
| 13 | Mid-sentence | "...and that was the moment {turn}." | "...and that day the bank pulled the loan. The factory had been open 3 days." |
| 14 | Flipped proverb | {Known saying, reversed.} | "The early bird gets nowhere." |
| 15 | Statistic | {N}% of {group} {surprising fact}. | |
| 16 | Verbatim question | "{Follower's question}" You ask this every week. | |
| 17 | Someone else's result | One {person} got {result} in {time}. | "One founder went from zero to {{result}} in {{time}}." |
| 18 | Superlative | The {fastest/biggest/only} {thing} is {answer}. | |

Rules: write the spoken line and the on-screen text separately (screen: 6 words or fewer). No intro; the video starts with the sentence that would normally arrive at second 6. Say the number ("a lot" is not a number). Deliver the hook's promise before the halfway point. Numbers come from a real source and are never invented; if unknown, leave `{{number}}` and flag it.

## Mode 1: Plan (weekly, same day)

Input: read the previous plan, swipe file and log notes if available (project files, Notion). Otherwise ask once: (1) the account's niche and 3–4 core themes, (2) the audience's country/time zone, (3) story or content candidates for this week and their sources, (4) 10 accounts the user wants to be seen by.

4–5 posts a week, at least 3 Reels (the only format that reaches non-followers). Carousels deepen existing followers. Don't put the same type back to back:

| Type | Per week | Job |
|---|---|---|
| Proof | 1 | a concrete result with a number. Reel |
| Lesson | 1–2 | one thing the viewer can apply today. Reel or carousel |
| Opinion | 1 | a position that might cost followers. Reel |
| Story | every 2 weeks | a scene with stakes, mini documentary. Reel |
| Series/Offer | every 2 weeks | the account's series, newsletter, collaboration call. Carousel or story |

For each slot: theme, this week's concrete angle (an angle, not a topic: "AI" is not a plan), format and hook formula number.

Timing: start from the audience's local morning commute (around 08:00–09:00) or evening (19:00–21:00) and adjust with the account's own data. Say it plainly: timing matters far less than the first two seconds. Optimising timing before the hooks land is polishing the wrong thing.

**Engagement round (required):** 20 minutes a day before posting, 10 accounts: 5 reach (have the audience you want, early comments get seen), 3 peers (similar size), 2 collaboration candidates. Commenting on the same 3 accounts daily looks like a bot; rotate the weekly list. Comments are 1–3 sentences, never open with "great post", never repeat the reel, never self-promote.

Output:
```
WEEK OF: 27 Oct
MON  engagement only (20 min)
TUE  08:30  REEL      PROOF    #4  Time collapse    - Ford assembly line
WED  story + engagement
THU  19:30  CAROUSEL  LESSON                        - Toyota's 5 Whys
FRI  08:30  REEL      OPINION  #3  Nobody tells you - ...
SUN  20:00  REEL      STORY    #13 Mid-sentence     - ...
STORY every day 3–5 frames, question box on Thursday
ENGAGEMENT (5 reach / 3 peers / 2 collabs): ...
Say "write Tuesday" and I'll draft it.
```
If a scheduling tool (Metricool, Buffer, Later...) is connected, offer to push the plan as drafts; nothing is scheduled without the user's approval.

## Mode 2: Research (monthly)

**Raw views are not evidence.** 400k views on a 2M-follower account is a quiet day; 400k on a 4k-follower account found something copyable. Everything is ranked by the **outlier ratio**: views / the median of that account's last 12 reels. Above 3× is signal; below 1.5× is that account's normal day.

1. **Pick accounts (6–12):** 4 direct (same niche, slightly ahead), 4 adjacent (different niche, same audience; borrow formats here), 2–4 large accounts (format only). Accounts within ~10× the user's size teach the most. The user's own "Saved" folder is the fastest corpus.
2. **Look:** through the user's signed-in browser if available, otherwise the user pastes screenshots/text. Never log in to Instagram on the user's behalf, ask for a password, or set up a scraper. This is reading, not scraping: 10 accounts, a dozen reels each.
3. **Record:** account | followers | median | views | hook (first sentence, verbatim) | first on-screen text | length | CTA.
4. **Rank and interpret:** compute the outlier ratio and give every hook a formula number. Report only three things: (a) formulas over-represented in the top third, with counts, (b) the structural common ground of the top third (hook length, is the first frame moving, is the payoff visual, where the CTA sits), (c) hooks that don't fit any formula (the most valuable column; it may be a new formula). State sample size and confidence: 40 reels from 6 accounts can carry a claim, 12 reels can't.
5. **Make it shootable:** for the top 3 formulas, write the hook line the user could say tomorrow with their own material. Never say "make a reel like this". Copy the formula, never the video: script, audio and edit are not copied, and every line is attributed to its source.

## Mode 3: Audit

Input: per-post insights (views, reach, non-follower reach %, 3-second hold, average watch time, saves, shares/sends, follows). Screenshots or a scheduling tool's report work. The retention graph of the best and worst reel is worth more than everything else.

Compute and show the working:
| Metric | Calculation | Meaning |
|---|---|---|
| Outlier ratio | views / account median | a real hit or a normal day |
| Non-follower reach | % | did it travel |
| 3-sec hold | still watching at 3s / started | the hook's grade |
| Average watch time | from insights | did the middle work |
| Sends per reach | shares / reach | the strongest signal you can earn |
| Follows per reach | follows / reach | did the profile convert attention |

Rank by outlier ratio and sends per reach, not by views. Put the top 5 and bottom 5 side by side and check, in order: 3-sec hold → hook formula → format → length (<15, 15–30, 30–60, 60+) → theme → were comments answered in the first hour → day/time (last, almost never the cause).

The key distinction: **a reel that got views but no follows is not a failed reel, it is a profile problem.** A reel nobody watched is a hook problem. If non-follower reach is high and follows per reach is low, stop writing hooks and fix the profile (name field, bio, 3 pinned posts, highlights).

Write each finding as a claim with its evidence and state your confidence; you can't see a pattern in 6 posts, and saying so beats inventing one. End with "STOP: ..." and "MORE: ..." and base the next plan on that evidence.

Credit: adapted from the `ig-plan`, `ig-viral`, `ig-audit` skills and `ig-reel/hooks.json` in github.com/Jakeschincariol/instagram-agent-skill (MIT); hook bank rewritten for third-person storytelling.
