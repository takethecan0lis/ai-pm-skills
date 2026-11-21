# Foundations: the ideas WSJF rests on

Each section gives what the idea is, how it connects to WSJF, and a source. Items marked "general background" have no fetched source in our notes; they are short and unattributed.

---

## Cost of delay

**What it is.** Per Wikipedia, "a way of communicating the impact of time on the outcomes we hope to achieve". It is measured in money per unit of time.

**How it connects.** It is the top half of the WSJF formula.

**Reported.** Wikipedia reports Reinertsen as saying about 85 percent of product managers do not know their cost of delay, and that intuitive estimates spread 50 to 1.

Source: https://en.wikipedia.org/wiki/Cost_of_delay

---

## Urgency profiles

**What it is.** Black Swan Farming describes four shapes of how delay costs value:

- short life cycle, where delay lowers the peak
- long life cycle, where delay lowers the peak
- long life cycle, where the peak is unaffected
- external deadline, where cost of delay is (quote) "zero until the point where you need to start development"

**How it connects.** It sits behind the time criticality column: a deadline and a fading market score differently.

Source: https://blackswanfarming.com/urgency-profiles/

---

## The economic view of product development

General background. Product work consumes scarce capacity, and the order you spend it in has a price. Reinertsen's 2009 book frames development decisions this way; we have not read it.

**How it connects.** WSJF is one way to make that price visible.

---

## Flow, queues and Little's Law

**What it is.** Little's Law says lead time equals work in progress divided by throughput. It holds only for a stable system. John Little published it in 1961. This is from a summary of the source; check the original before relying on it.

**How it connects.** Waiting time in queues is where cost of delay piles up, and the law shows why more work in progress means longer waits.

Sources: https://businessmap.io/continuous-flow/littles-law and https://kanban.university/wp-content/uploads/2022/09/Exploring-Littles-Law-KGS-2022.pdf

---

## Shortest job first in scheduling

General background. In scheduling theory, running the shortest job first reduces average waiting time when all jobs are equally valuable. The weighted form is known as Smith's rule (1956).

**How it connects.** WSJF adds weights (value) to that idea: short and valuable first.

---

## Relative estimation and planning poker

**What it is.** Scoring items against each other on a Fibonacci-style scale, rather than in hours or money. Both appear on the SAFe WSJF page.

**How it connects.** It is how WSJF columns get filled when no money figures exist.

Source: https://webarchive.library.unt.edu/web/20161225031923mp_/http://www.scaledagileframework.com/wsjf

---

## Opportunity cost and time value

General background. Doing one thing means not doing another, and value now differs from value later. Wikipedia's cost of delay page carries a finance example of time value.

**How it connects.** Both explain why waiting has a price at all.

Source: https://en.wikipedia.org/wiki/Cost_of_delay

---

## Kanban classes of service

**What it is.** Expedite, fixed date, standard and intangible, each tied to a cost-of-delay shape. Expedite may break WIP limits. Without cost of delay, the classes slide into subjective urgency calls. This is from a summary of the source; check the original before relying on it.

**How it connects.** It treats cost-of-delay shape as a rule for how work is handled, where WSJF uses it as a score.

Sources: https://businessmap.io/kanban-resources/getting-started/kanban-classes-of-service and https://www.scrum.org/resources/blog/classes-service-kanban-what-are-they

---

## Lean portfolio management and PI planning

**What it is.** SAFe practices where WSJF is used to order epics and features. This is from a summary of the source; check the original before relying on it.

**How it connects.** They supply the setting in which WSJF scores get discussed.

Source: https://agility-at-scale.com/safe/lpm/wsjf-weighted-shortest-job-first/

---

## HiPPO and decision rights

**HiPPO.** The highest paid person's opinion. Korzec, writing for the SEI, names it as a risk of committee-based prioritization, which WSJF scoring sessions often are (our reading): one voice dominating the scoring. Source: https://sei.cmu.edu/blog/mission-based-prioritization-new-method-sequence-features-capabilities-and-epics

**Decision rights.** General background. Who gets to decide what.

**How they connect.** The sponsor-scores-cost-of-delay variation is one attempt to set decision rights: the sponsor owns value, the team owns size.

---

## Sunk cost

**What it is.** Money or effort already spent. The SAFe WSJF page says it is ignored, because only the remaining size is estimated.

**How it connects.** It keeps old investment from skewing the order.

Source: https://webarchive.library.unt.edu/web/20161225031923mp_/http://www.scaledagileframework.com/wsjf

---

## Batch size

General background. Smaller batches move through a system faster and give feedback sooner.

**How it connects.** The SAFe page says big jobs may need splitting so they can compete in the ranking.

---

## Sources

- https://webarchive.library.unt.edu/web/20161225031923mp_/http://www.scaledagileframework.com/wsjf
- https://en.wikipedia.org/wiki/Cost_of_delay
- https://blackswanfarming.com/urgency-profiles/
- https://businessmap.io/kanban-resources/getting-started/kanban-classes-of-service (summary only)
- https://www.scrum.org/resources/blog/classes-service-kanban-what-are-they (summary only)
- https://businessmap.io/continuous-flow/littles-law (summary only)
- https://kanban.university/wp-content/uploads/2022/09/Exploring-Littles-Law-KGS-2022.pdf (summary only)
- https://agility-at-scale.com/safe/lpm/wsjf-weighted-shortest-job-first/ (summary only)
- https://sei.cmu.edu/blog/mission-based-prioritization-new-method-sequence-features-capabilities-and-epics

Adopted, not measured: this page explains a method and reports what the sources say; it claims no result of its own. CC BY 4.0. Attribution: Drew Podwal.
