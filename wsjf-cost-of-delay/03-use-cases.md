# Use cases

Six cases as the sources report them. We have not verified any of them. Items from a search snippet are marked "from a summary of the source; check the original before relying on it".

---

## 1. Epics at a railway company

**Situation.** A SAFe transformation at a German railway company ranked business epics with WSJF. From a summary of the source; check the original before relying on it.

**Inputs.** Not reported.

**What the source reports.** That WSJF was used. The page reports no WSJF-specific numbers.

**What this does not show.** Any result of the ranking, or how the scores were set.

Source: https://scaledagile.com/blog/region/europe/page/2 (listing page; the post may have moved)

---

## 2. A defence program's backlog

**Situation.** A US Department of Defense program, per Korzec at the SEI (2020-11-12), had 178 portfolio epics and more than 900 features.

**Inputs.** Korzec reports that full reprioritization with WSJF was dropped, so the backlog lost its order, and that a replacement method was tested by a 19-person group that spent about 2 hours on weights and about 1 hour on 55 features. Korzec counts 400 comparisons for 100 items.

**What the source reports.** WSJF was hard to keep up at that size, and Korzec says it did not fit his features. It was a case where WSJF was set aside.

**What this does not show.** That the replacement method beats WSJF in general; the test was one group and 55 features.

Source: https://sei.cmu.edu/blog/mission-based-prioritization-new-method-sequence-features-capabilities-and-epics

---

## 3. A fixed-date regulatory item (teaching example)

**Situation.** An illustrative migration with a regulatory date. A teaching example, not a reported outcome. From a summary of the source; check the original before relying on it.

**Inputs.** The source scores value 8, time criticality 13, risk reduction 5, giving cost of delay 26. Size 5 gives WSJF 5.2.

**What the source reports.** The arithmetic only.

**What this does not show.** A real result. Where a legal deadline is the only thing that matters, the score adds little.

Source: https://agility-at-scale.com/safe/lpm/wsjf-weighted-shortest-job-first/

---

## 4. Tech debt scored as an enabler

**Situation.** Technical work with no direct user value.

**Inputs.** One source scores it on project value, not user value. Another uses relative risk-reduction scoring for authentication against profile features. Both from a summary of the source; check the original before relying on it.

**What the source reports.** That enabling work can be scored in the risk reduction and opportunity enablement column.

**What this does not show.** Any outcome, or how scores were agreed.

Sources: https://subscription.packtpub.com/book/iot-and-hardware/9781803235820/1/ch01lvl1sec12/work-item-prioritization (may require sign-in) and https://www.insights.cgi.com/blog/what-is-wsjf-how-to-use-this-agile-concept-to-prioritize-work

---

## 5. Cost of delay without WSJF (Maersk Line)

**Situation.** Black Swan Farming reports that one feature at Maersk Line waited 38 weeks in queues.

**Inputs.** Black Swan Farming gives cost of delay above $200,000 a week.

**What the source reports.** Close to $8 million lost, as Black Swan Farming states it.

**What this does not show.** WSJF scoring. It is a cost-of-delay example only. The figures are Black Swan Farming's own; we checked them against their page.

Source: https://blackswanfarming.com/cost-of-delay/

---

## 6. LLM request scheduling (not backlog ordering)

**Label: request scheduling, not backlog ordering.**

**Situation.** EWSJF is a scheduler for LLM requests in vLLM. It orders requests, not work items.

**Inputs.** Not described here.

**What the source reports.** The paper's abstract reports more than 30 percent higher throughput and up to 4x faster first token for short requests. From a summary of the source; check the original before relying on it. Not verified by us.

**What this does not show.** Anything about ordering a human backlog. We found no published source of agents ordering their own queues with WSJF.

Source: https://arxiv.org/abs/2601.21758

---

## When not to use WSJF

- When value is not economic, such as government missions. Korzec argues government missions are measured by mission impact, not profit (SEI, Korzec).
- When the backlog is too large to re-score each time it changes (SEI, Korzec).
- For small items where duration is unknowable (from a search summary; check the original before relying on it).
- For items that realize no value on release (PMI; from a summary of the source; check the original before relying on it).
- When resources are not fixed, because size then misleads (SAFe 2016 page).
- When ordinal scores are treated as real numbers (from a summary of the source; check the original before relying on it).
- When one senior voice dominates the scoring (HiPPO risk, SEI, Korzec).

Use WSJF to start a conversation, not as arithmetic. That is our judgment, not a finding.

---

## Questions to ask before you score

- Is the value economic, or something else?
- Are resources fixed enough that size means duration?
- Is the list small enough to re-score when facts change?
- Who scores which column, and does anyone score their own item's size?
- Is there a fixed date that makes the score moot?
- What will you write down beside each score: date, inputs, assumptions?
- Will you treat near-ties as ties?

---

## Sources

- https://scaledagile.com/blog/region/europe/page/2 (summary only; listing page; the post may have moved)
- https://sei.cmu.edu/blog/mission-based-prioritization-new-method-sequence-features-capabilities-and-epics
- https://agility-at-scale.com/safe/lpm/wsjf-weighted-shortest-job-first/ (summary only)
- https://subscription.packtpub.com/book/iot-and-hardware/9781803235820/1/ch01lvl1sec12/work-item-prioritization (summary only; may require sign-in)
- https://www.insights.cgi.com/blog/what-is-wsjf-how-to-use-this-agile-concept-to-prioritize-work (summary only)
- https://blackswanfarming.com/cost-of-delay/
- https://arxiv.org/abs/2601.21758 (summary only)
- https://webarchive.library.unt.edu/web/20161225031923mp_/http://www.scaledagileframework.com/wsjf
- https://www.pmi.org/disciplined-agile/improving-wsjf (summary only)

Adopted, not measured: this page explains a method and reports what the sources say; it claims no result of its own. CC BY 4.0. Attribution: Drew Podwal.
