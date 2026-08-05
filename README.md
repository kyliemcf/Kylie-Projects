# 13.1 — Half Marathon Training

A two-person training tracker built around **Hal Higdon's Novice 1 half marathon
program** — 12 weeks, 206.4 miles, ending at 13.1.

It's a single self-contained `index.html`. No build step, no server, no account.
Open the file (or the published link) in any browser, add it to your phone's home
screen, and it behaves like an app.

## What's in it

**Three tracker bars, always visible**

| Bar | Shows |
| --- | --- |
| Today | Miles logged against today's prescribed workout |
| This week | The week's running total against that week's plan |
| All 12 weeks | Everything you've run against the full 206.4 |

**A little runner on every bar.** It stands at your current progress and runs as
you log miles. Hit a goal and it throws its arms up, turns orange, and jumps
while confetti goes off.

The celebration is tiered on purpose:

- **Runs and races** — confetti, the jumping runner, and a message
- **Cross-training** — a quiet acknowledgement, no confetti
- **Rest days** — nothing. Resting is on the plan, not an achievement

Each goal celebrates exactly once, ever. It won't re-fire when you reload.

**Two runners.** Switch between the two profiles at the top; each keeps its own
log. The "Both of you" panel shows where you each stand this week and overall.

**Log any day, not just today.** Tap any day in the week strip or anywhere in the
full 12-week table to log or backfill it. Wednesdays are "run or cross" in this
plan, so those days have a *Crossed instead* button.

## The plan

Hal Higdon's Novice 1: Monday rest, runs Tuesday/Wednesday/Thursday, Friday rest,
cross-training Saturday, long run Sunday. It builds from 3-mile runs in Week 1 to
a 10-mile long run in Week 11, with a 5-K in Week 6 and a 10-K in Week 9, then
tapers into race day.

Races count toward mileage at 3.1 / 6.2 / 13.1. Cross-training days are
time-based, so they're marked done rather than adding miles — which is why a
"complete" week can still be 100% with cross days on it.

Source: <https://www.halhigdon.com/training-programs/half-marathon-training/novice-1-half-marathon/>

## Setup

Open **Setup & sync** at the bottom.

- **Week 1 Monday** — set this to the Monday you start. Everything (which week
  you're in, the race-day countdown) is derived from it. Race day is the Sunday
  of Week 12.
- **Runner names** — rename the two profiles to whatever you like.

## About syncing

Your data is saved in that browser's local storage and is never uploaded
anywhere. It does **not** sync between devices on its own.

To move everything to another phone: **Copy code** on the first one, paste it
into the box on the second, press **Load**. That transfers both runners' full
history. Re-copy whenever you want to bring them back in line.

If you both want to see each other's live progress without copying codes, that
needs a backend this deliberately doesn't have.

## Running it

Open `index.html` in a browser. That's it — nothing to install.
