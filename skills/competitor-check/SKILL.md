---
name: competitor-check
description: Compare an Instagram account with the accounts it tracks in Synclify. Use when the person asks how they stack up against competitors, what a competitor is doing, or what to do differently.
---

# Competitor check

## Steps

1. Call `get_competitors` for the accounts being tracked and where this account stands among them.
2. For one named account, call `compare_to_competitor`.
3. For how the tracked accounts make their posts (formats, lengths, hooks), call `get_competitor_patterns`. For their individual posts, call `get_competitor_content`.
4. For what to do about it, call `plan_against_competitors`.

## How to answer

- Say which accounts the comparison covers and over what period.
- Separate what the tools measured from what they could not. Instagram does not share another account's reach or saves, so comparisons rest on public numbers such as likes, comments, views and how often they post.
- Finish with two or three specific moves, each tied to something a tool returned.

If the account tracks nobody yet, say so. Tracking a new account is done with `manage_competitors`, which asks for a yes before it starts.
