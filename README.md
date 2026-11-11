# Synclify for Claude

Puts your whole Instagram in one place: content, DMs, brand deals, invoices, analytics. You ask, the assistant does it, and it checks with you before it changes anything.

This plugin connects Claude to your Synclify account and adds four skills for the jobs people do most often.

## What you need

- A Synclify account on a paid plan. Sign up at https://synclify.ai.
- A professional Instagram account (business or creator) connected inside Synclify.

## What it does

Once it is connected you can ask Claude things like:

- How did my reels do this week?
- Which of my last ten posts brought the most followers?
- Plan next week's posts around my three best topics.
- Who still owes me money, and which deals are at risk?
- What are the accounts I track doing that I am not?

The skills in this plugin:

| Skill | When Claude uses it |
| --- | --- |
| `weekly-review` | You ask how the account did this week or this month |
| `plan-content-week` | You ask for a content plan, post ideas for the week, or what to post next |
| `deals-and-invoices` | You ask about brand deals, what you are owed, or chasing a late payment |
| `competitor-check` | You ask how you compare with accounts you track |

## What it connects to

The plugin declares one remote server, Synclify's own, at `https://app.synclify.ai/mcp/directory`. Claude sends you to Synclify to sign in and approve the connection. Nothing else is contacted, nothing is installed on your computer, and the plugin runs no scripts or hooks.

Every tool is marked as either reading or changing. Reading tools only look at your account. Changing tools save drafts, plans, notes and settings, and ask you first before anything that leaves your workspace, such as scheduling a post. Publishing, sending messages and spending money are done in Synclify itself, where you can confirm and undo them.

Video editing and AI image, video and voice generation are not part of this plugin. They are done in the Synclify app.

## Your data

Claude sees only what a tool returns for the question you asked. Synclify does not read your Claude chats, memory or files. You can disconnect at any time in Claude, or in Synclify under Settings, where every connected app is listed with when it was last used.

Privacy policy: https://synclify.ai/privacy

## Help

Setup guide: https://synclify.ai/apps/claude

Support: support@synclify.ai

## License

MIT. See `LICENSE`.
