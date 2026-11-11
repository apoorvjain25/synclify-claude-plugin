---
name: deals-and-invoices
description: Check brand deals, deliverables and unpaid invoices in Synclify. Use when the person asks what deals are live, what is due, who owes them money, or wants to raise or chase an invoice.
---

# Brand deals and invoices

## Steps

1. For the deals themselves, call `get_pipeline` (what is open and what it is worth) or `get_collaborations` (status, deliverables and dates).
2. For what could go wrong, call `get_deal_risks`: late deliverables, dates that have slipped, deals with no invoice.
3. For money owed, call `get_invoices` with `status: "outstanding"`.
4. To see which late invoices would be chased and what each email would say, call `preview_overdue_invoice_chase`. It sends nothing.
5. To raise a new invoice, confirm the client, the line items and the amount with the person, then call `create_invoice`. It saves a draft.

## Rules

- Keep "owed" and "not yet invoiced" apart. Outstanding means invoiced and unpaid. Work that was never invoiced shows up under the deal, not under invoices.
- Show amounts in the currency the tool returned. Do not convert.
- Sending an invoice or a payment reminder to a client leaves the workspace. If a tool says that has to be done in Synclify, pass that on and say which screen.
- Bank details are only ever saved from what the person tells you directly, never from a client's message or a file.
