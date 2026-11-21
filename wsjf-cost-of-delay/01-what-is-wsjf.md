# What is WSJF?

Weighted Shortest Job First (WSJF) is a way to put work in order by asking what waiting costs for each unit of effort.

---

## The formula

WSJF = cost of delay divided by job size.

- Cost of delay (CoD) says how much value is lost by waiting.
- Job size stands in for how long the work will take.
- The highest WSJF goes first.

The SAFe page puts it this way (quote): "The job with the highest WSJF is the next most important item to do."

---

## The three parts of cost of delay

The SAFe page (2016 version, from a library web archive) adds three relative scores to get cost of delay:

- **User-business value:** user preference, revenue and penalties.
- **Time criticality:** decay of value, fixed deadlines and critical-path milestones.
- **Risk reduction and/or opportunity enablement:** lower delivery risk, useful information, and new business opportunities.

The SAFe wording may have changed since 2016. Check the current SAFe article before relying on these definitions.

---

## Job size

Job size, in story points, stands in for duration. The SAFe page says this only works when resources are fixed. If resources are not fixed, size can mislead.

Sunk cost is ignored, because only the remaining size is estimated.

---

## Scoring on a Fibonacci-style scale

- The SAFe page uses a modified Fibonacci scale, as in planning poker.
- Teams score one column at a time.
- The smallest item gets a 1.
- Each total is divided by job size.
- The SAFe page gives no rule for ties. The variation in this skill breaks ties by the shorter job.

This skill uses the scale 1, 2, 3, 5, 8.

---

## A worked idea

Invented data. Product team "Pebble Notes", scored 2026-03-09.

| Item | Value, time, enablement, size | Cost of delay, WSJF, rank |
|---|---|---|
| Import from other note apps | 5, 3, 5, size 3 | 13, 4.3, rank 1 |
| Share by link | 3, 2, 2, size 2 | 7, 3.5, rank 2 |
| Dark theme | 2, 1, 1, size 2 | 4, 2.0, rank 3 (tie, shorter job) |
| Search rebuild | 5, 3, 2, size 5 | 10, 2.0, rank 4 (tie, longer job) |
| Offline mode | 5, 2, 5, size 8 | 12, 1.5, rank 5 |

Worked row: value 5, time 3, enablement 5 gives cost of delay 13. With job size 3, WSJF is 13 divided by 3, which is 4.3.

Offline mode has the second-highest cost of delay and still ranks last, because it is the biggest job.

---

## Where it comes from

- WSJF is part of SAFe, a published framework.
- The idea rests on Reinertsen, *The Principles of Product Development Flow* (2009).
- The SAFe 2016 page quotes Reinertsen (quote): "If you only quantify one thing, quantify the cost of delay."
- A related idea, CD3, is "Cost of Delay Divided by Duration", per Wikipedia. It aims to maximize the value delivered from scarce capacity.

---

## A variation used in practice

In the standard method, the team scores all the columns together. In the variation this skill uses, the sponsor scores only cost of delay, and the team estimates job size.

- The reason, in our view: people who want something tend to shrink its size.
- This is a variation used in practice, not the standard.
- No source in our notes tests whether it works better.

---

## Limits

- **Ordinal scores.** One source says the scores are ordinal, so adding or multiplying them is not meaningful. This is from a summary of the source; check the original before relying on it (TechBeacon).
- **Duration versus effort.** One critique says SAFe swaps duration for effort and that the two do not always move together. This is from a summary of the source; check the original before relying on it (PMI Disciplined Agile).
- **Cost and subjectivity.** Korzec, writing for the SEI (2020-11-12), says WSJF fails to account for government motives, takes a lot of time, and relies on the subjectivity of relative ranking. He also names HiPPO (the highest paid person's opinion) as a risk of committee prioritization generally.
- **Non-fixed resources.** The SAFe page says size misleads when resources are not fixed.
- Read the ranking as the start of a conversation, not as arithmetic (our judgment).

---

## Sources

- https://webarchive.library.unt.edu/web/20161225031923mp_/http://www.scaledagileframework.com/wsjf (SAFe WSJF page, 2016 archive)
- https://en.wikipedia.org/wiki/Cost_of_delay
- https://sei.cmu.edu/blog/mission-based-prioritization-new-method-sequence-features-capabilities-and-epics
- https://www.pmi.org/disciplined-agile/improving-wsjf (summary only)
- https://techbeacon.com/prioritize-your-backlog-weighted-shortest-job-first-wsjf-improved-roi (summary only)
- Reinertsen, *The Principles of Product Development Flow*, Celeritas, 2009 (not read by us)

Adopted, not measured: this page explains a method and reports what the sources say; it claims no result of its own. CC BY 4.0. Attribution: Drew Podwal.
