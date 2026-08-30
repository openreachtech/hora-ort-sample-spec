<!-- 日本語版: [README.ja.md](./README.ja.md) — 片方を直したら、同じコミットでもう片方も直してください -->

# Expense note

An internal expense sheet, for one company. A member of staff signs in with an account somebody issued them, records what they paid — the date, the amount, a category and a memo — corrects or removes their own entries, and reads one month at a time with its total.

Nobody sees anybody else's entries, there is no approval, and there is no manager. That is the whole product, and it is deliberately that small.

## The spec

[`specs/1.0.0/spec.md`](./specs/1.0.0/spec.md) — 349 lines, three features, seven operations, three screens.

**It is the document `/hora-spec` wrote, as it wrote it.** Nothing was tidied up afterward.

## What it took to write

**Stage 0 read nothing**, because there was nothing to read: a fresh project, no repository, no document, and the request stated in conversation rather than dropped into `request/`.

**Four questions were put before stage 1 began** — whether any document existed somewhere the session could not reach, how many kinds of user there are, how a user gets an account, and which language `/hora` writes questions in. Three answers shaped the document:

- **one actor.** A member of staff, managing their own expenses
- **accounts are issued by an operator**, outside the product. So there is no sign-up screen, no administrator actor, and the `Actors and roles` table has one row
- **questions in English**

Everything else went out as a proposal and was approved: the three features, every use case, every acceptance criterion, the data model, the operations and the screens.

## What the run decided, and where to look for it

| | Where |
|---|---|
| **Reading one's own entries belongs to `#expense-entry`, not to `#monthly-summary`** — the other way round, `#expense-entry`'s use cases would name a feature built after it, which `/hora-plan` stops on | sections 11 and 12 |
| **Three things deferred, each with the seam it needs named** — a `status` column from the first migration for approval, one operation returning both a month's entries and its total for the export, a category as a row rather than an enum | section 4 |
| **No background job, so no Redis** — every write finishes inside its own request | section 8 |
| **One endpoint, one identity model**, with the reason written down: a manager in 1.1.0 is a role on the same login, not a second server | sections 2 and 7 |
| **Another member of staff's expense is answered as not found, never as forbidden** | sections 11 and 12 |

## Status

**The spec is written; the build has not run yet.** What is published here is the output of `/hora-spec` alone.
