---
name: weekly-review
description: Review how an Instagram account did over the last week or month using Synclify. Use when the person asks how their account, posts or reels did, whether they are growing, or what worked recently.
---

# Weekly review

Use the Synclify tools to answer with the account's own measured numbers.

## Steps

1. Call `review_my_week` for the last seven days against the seven before. For a longer window, call `get_period_comparison` with the period they named.
2. Call `get_top_content` for the same period to find the posts that did best, ranked by the metric they care about (reach if they did not say).
3. Call `explain_what_worked` to see which attributes of their posts go with the better results.
4. If followers are the question, call `diagnose_growth`.

## How to answer

- Lead with the one or two things that changed most, then the posts behind them.
- Name each post so they can find it, and say which number it is ranked on.
- If a tool says something was not measured, say that. Do not fill the gap with an estimate or a zero. `get_data_coverage` explains why a field is empty.
- End with one concrete thing to try next week, taken from what the tools returned.

Everything in this skill reads only. Nothing is changed on the account.
