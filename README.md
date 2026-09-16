# calendar-context

The "context brain" for an automated calendar groomer. The single file, `context.md`, is the instruction set the groomer reads before it renames and categorizes events on my Google Calendar.

## What's in `context.md`

- **Who I am** — framing for the groomer (work and personal share one calendar; treat both as first-class).
- **Category definitions** — the fixed taxonomy every event is sorted into (Call, Workout, Work Time Block, Self Care, Hangout, Transit time, Meal Break, Content Creation, Mental Exercise/Instrument, Plan the next day, Life Time) with tie-break rules.
- **Title conventions** — the required format `Category: Descriptive Title — Duration`, with before/after examples.
- **Recurring blocks, people, firms, vendors, shorthand** — reference lists so the groomer expands abbreviations and names correctly instead of inventing them.
- **Do not touch** — events the groomer must leave alone.

## How it's used

The groomer loads the current `context.md` as its starting point on every run, and the file itself is rewritten automatically every Sunday with what it learned that week. Hand edits are welcome at any time — they get absorbed into the next rewrite. The one hard rule encoded here is that the groomer must never invent a name, company, figure, or detail that isn't in the input.
