---
name: plan-content-week
description: Plan a week of Instagram posts with Synclify and put the ones the person approves on their calendar. Use when they ask for a content plan, post ideas for the week, or what to post next.
---

# Plan a week of content

## Steps

1. Call `get_calendar` for the coming week so the plan fits around what is already there.
2. Call `get_pillars_tags_collections` for the topics the account posts about, and `get_best_posting_times` for the slots that have worked for it.
3. If they want ideas first, call `generate_content_ideas` and let them pick.
4. Call `plan_week` with what they asked for. It returns a dated plan: what to post, on which day, with the hook, caption and ask for each.
5. Show the plan as a short list by day. Ask which posts they want to keep.
6. For each post they keep, call `create_content_draft` to save it, then `schedule_content` to give it a date and time. `schedule_content` answers with what it will do first and acts only when called again with `confirmed: true`, so make that second call only after they say yes.

## Rules

- Ask before saving or scheduling. Reading tools need no permission; the tools marked as changing do.
- Publishing itself happens from Synclify at the scheduled time. If they want to post right now, tell them to do it in the Synclify app.
- Keep to the topics and times the tools returned. If the account has too little history for posting times, say so.
