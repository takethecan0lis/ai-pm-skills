---
name: not-verified-build-report
description: Writes a four-part report whenever a change is handed over for testing or review: what changed, what is verified with evidence, what is NOT verified (this part is never empty or left out), and decisions for the owner. The report names the build by hash or version. Use when finishing a change, feature or fix and about to say it is done, ready or working, and whenever a handover tends to overclaim.
---

# Not-verified build report

## Purpose
"Done" often means "I built it". This skill forces a handover to say what was actually checked and what was not, so the owner tests the right things and nobody trusts an unchecked claim.

## Objective and benefit
**Objective:** Every report says what was checked, what was not, and what is needed from the owner.

**Benefit:** "Done" is less likely to mean "looks done". Gaps are easier to see before release, and the owner can judge the evidence instead of trusting a claim. Without it, an unchecked area ships as if it had been tested, and the first person to find the problem can be a user.

**Why it is worth having:** It helps keep status honest, which is what lets an owner decide what to test next. The aim is fewer surprises after release.

## When to use
- You are handing a change to someone who will test, review or accept it.
- You are about to write "done", "ready" or "working".
- Only one finished build should wait on its owner at a time. If another is already waiting, finish that handover first.

## Steps
1. Name the build at the top: a version number or a short commit hash. If it has neither, say so and give the date and time.
2. Part 1, What changed: two to five plain lines on behavior the owner would notice. No code walkthrough.
3. Part 2, What is verified, with evidence: for each claim, name the check and where its output lives (a test result, a screenshot, a log line, a record count). A claim with no evidence moves to part 3.
4. Part 3, What is NOT verified: list every area you did not check and the reason (no time, no access, no test data, depends on another team). This part is never empty and never omitted. If you believe everything was checked, write what the checks could not see, such as real users, real volume or other browsers.
5. Part 4, Decisions or tests for the owner: at most 3 lines, each a decision or a test the owner must do, recommended answer first.
6. Use plain status words. "Built" means it exists, "tested" means a check ran and passed, "verified" means evidence is attached. Do not use "done" for anything not run.
7. Freeze the build before anyone reviews it. If a reviewer finds problems, fix them in one batch and issue a new build name rather than patching the old report.

## Example
Invented data. Product team "Pebble Notes", build 2.4.1 (hash a3f9c21), 2026-03-12.

1. What changed: new users now see a three-step checklist after signup. Skipping the checklist is remembered for 30 days.
2. Verified: checklist shows for a new test account (screenshot attached); skip is remembered after logout (test log, 3 of 3 passed); 12 automated tests for the checklist pass (run log).
3. NOT verified: behavior on Safari and on phones under 5 inches; accounts created before 2026-01-01; behavior with 10,000 or more simultaneous signups; the English copy was not reviewed by the content owner.
4. For you: approve the copy on the second step (recommended: approve as written). Test one older account on your phone before release.

## What this does not verify
- It does not make the checks good; a weak test can still be listed as evidence. The owner judges the evidence.
- It cannot catch what the author does not know to list as unverified.
- Adopted, not measured: no result is claimed for fewer escaped defects or faster acceptance.

## Licence and version
CC BY 4.0. Attribution: Drew Podwal. Version 0.1, 2026-11-21. Adopted, not measured.
