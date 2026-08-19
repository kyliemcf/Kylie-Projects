# Pace Ourselves

A two-person half marathon training app for Kylie and Caleb, built around **Hal
Higdon's Novice 1 program** — 12 weeks, 199.4 miles, ending at 13.1 on
**Thursday, November 26 2026**.

It's a single self-contained `index.html`. No build step, no server, no account.
Open the file (or the published link) in any browser, add it to your phone's home
screen, and it behaves like an app.

## Screens

It opens on a **home screen** asking who's running today. Pick Kylie or Caleb —
each card shows that runner's character and how far through the plan they are —
and the app signs you in. You stay signed in until you tap your name in the top
bar to switch back.

Three tabs along the bottom:

| Tab | What's on it |
| --- | --- |
| **Log** | Today's mileage bar *and* the whole-plan bar, the day you're logging, and the journal |
| **Week** | This week's mileage bar, the seven-day strip, and an editor for which days you run |
| **Plan** | Overall progress across all 12 weeks, both runners side by side, the full plan table, and setup |

The three tracker bars — today, this week, all 12 weeks — are spread across the
tabs so the number matches the screen you're on, except the whole-plan bar, which
appears on both Log and Plan: while you're logging a run it's useful to see the
day's goal and how far through the 199.4 you are together. Both copies are the
same meter and move in step.

Everything cross-links: tap a day in the week strip or anywhere in the plan
table and it opens on the Log tab ready to enter miles.

**A journal on every day.** Under the day you're logging there's a note field
that asks the right question for that day — *How did the run feel?*, *Rest day —
how did recovery go?*, *How did the race go?* — with a placeholder to get you
started. It saves as you type.

Earlier entries collect below, newest first, each showing the date, the workout,
the miles and what you wrote. Days you logged miles on but haven't written about
still appear, so the journal doubles as the full record of everything you've run
— tap one to add a note. Notes and miles are stored independently: clearing a
day's miles never deletes what you wrote about it.

**A little runner on every bar.** A plain stick figure — it stands at your current
progress and runs as you log miles. Hit a goal and it flings its arms out, turns
mint green, and jumps while confetti goes off. Kylie's has a ponytail that hangs
at rest and streams back as she runs; Caleb's wears a cap. The character follows
whichever profile is selected.

**Hitting a goal throws a party.** Confetti erupts from the runner itself — or
from the day card if you're backfilling an earlier day — arcing up and tumbling
down, the bar flashes mint, the number pops, and a message slides in. Finishing a
week or the whole plan gets a bigger, double burst.

A goal celebrates every time you *cross* it, so clearing a day and re-logging it
celebrates again. Piling extra miles on top of a goal you've already met doesn't
re-fire, and neither does reloading the page — only the moment you go from unmet
to met counts.

Only mileage is celebrated. Rest days get nothing — resting is on the plan, not
an achievement. (Which is why opening the app on a rest day looks quiet: mark it
*Rested* and it just ticks off.)

**Two runners.** Each keeps its own log, its own arrangement of days, and its own
character. The "Both of you" panel on the Plan tab shows where you each stand.

**Log any day, not just today.** Step through days with the arrows on the Log
tab, or tap any day in the week strip or the full plan table.

**Reshape any week around your life.** The Week tab's **Which days you run**
section lists all seven days, each with a picker holding that week's workouts.
Travelling Friday to Sunday? Set Monday to the 3-miler and Thursday to the long
run, and the rest days move to the days you're away. A few things worth knowing:

- Choosing a workout for a day swaps it in from wherever it currently sits, so
  the week's mileage is identical however you arrange it
- Miles you've already logged stay on the date you actually ran them; only the
  plan moves
- Identical workouts are listed once — the three rest days are interchangeable,
  so the picker doesn't repeat them
- Each of you rearranges independently; Kylie's travel week doesn't touch Caleb's
- A rearranged week is labelled as such, and **Reset week** puts it back to
  Higdon's shape without touching anything you've logged

## The plan

Hal Higdon's Novice 1 mileage, rearranged to be **miles only** — no
cross-training anywhere:

| Mon | Tue | Wed | Thu | Fri | Sat | Sun |
| --- | --- | --- | --- | --- | --- | --- |
| Rest | Run | Run | Rest | Run | Rest | Long run |

Four runs a week, three rest days. Against Higdon's original that means his
Wednesday "run or cross" is just a run, his Thursday run moves to Friday, and his
Saturday cross-training is gone. **Weekly mileage is unchanged**, since the cross
days never carried any miles to begin with.

It builds from 3-mile runs in Week 1 to a 10-mile long run in Week 11, with a 5-K
in Week 6 and a 10-K in Week 9, then tapers into race day.

**Race day is a Thursday, and Higdon's plan races on a Sunday.** Rather than
sliding the whole calendar (which would drag every long run onto a Thursday),
weeks 1–11 stay on their Mon–Sun grid so long runs stay on the weekend, and week
12 is a short week: Monday to race day. It takes the tail of Higdon's taper, so
the days immediately before the race are exactly the ones he prescribes —
2 mi, rest, rest, race. That makes week 12 worth 15.1 miles and the plan 199.4.

Working back from November 26, **Week 1 Monday is September 7 2026**.

Races count toward mileage at 3.1 / 6.2 / 13.1.

Source: <https://www.halhigdon.com/training-programs/half-marathon-training/novice-1-half-marathon/>

## The look

A training instrument that still has a pulse. Hairline borders and a disciplined
neutral scale carry the layout; a single rose accent is spent only where it means
something — progress fill, the figure you're chasing, today's date. Green is
reserved for completion, amber for race days, so colour always says something.

**Every number is set in a tabular monospace** while the interface text is a
system sans. Columns of miles line up down the plan table, figures don't jitter
as they tick over, and the whole thing reads like a log book rather than a
dashboard.

Radii are a scale — 6 / 10 / 14 — with full pills reserved for the tab bar and
status tags, so roundness signals something instead of being everywhere at once.

The wordmark stacks **Pace / Ourselves.** over two lines and ends on a rose full
stop; the 13.1 sits in the subtitle with the rest of the plan details.

Both themes are designed rather than inverted: light is a cool paper white with
white cards, dark is a near-black with lifted surfaces and brighter accents.

## Setup

Open **Setup & sync** at the bottom.

- **Race day** — set to November 26 2026. Everything else is derived from it:
  Week 1 Monday, which week you're in today, and the countdown. Change the date
  and the whole plan re-anchors, including the shape of week 12.
- **Runner names** — rename the two profiles to whatever you like.

Rest days can still be marked done, and any day accepts bonus miles if you run
when the plan says rest — those count toward your weekly and overall totals.

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
