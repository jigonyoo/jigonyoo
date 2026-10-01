### Jigon Yoo

I build defect-detection tools and publish the catch rate rather than assert it.
Every figure below sits in a public MIT repository beside the script that produced it.

| What it catches | Measured | Repository |
|---|---|---|
| Side effects that execute twice | 40 concurrent OS processes racing one refund — **20/20** deterministic detections of two reclaim-path defects that a statistical race test passed | [once-guard](https://github.com/jigonyoo/once-guard) |
| Prompt injection, tested against itself | **26/26** on the corpus written *for* it — **5/42** on the corpus written to *break* it | [llm-guardrails](https://github.com/jigonyoo/llm-guardrails) |
| Airflow DAGs, parsed instead of imported | **12/12** planted defects caught, **0** false positives on the clean DAG | [dag-guard](https://github.com/jigonyoo/dag-guard) |
| Loads that exit zero and are still wrong | a sabotaged batch fails **12** contract tests; the clean batch passes with **0** — the batch it stops reports $4,905,051 of revenue with zero load errors, $4.5M of it from one row | [warehouse-quality-gate](https://github.com/jigonyoo/warehouse-quality-gate) |

**The 5/42 is the number I lead with.** A filter tested only against the corpus
written for it has not been tested. Both corpora are published, so the bad
number is reproducible in one command rather than quoted.

---

**Documentation is a review surface too.** I numbered all 158 behavioural claims
in one README and tried to produce the command proving each: **7 were wrong, 18
had nothing behind them.** I deleted the latency figures I could not reproduce
and published the correction rather than dropping them quietly.

**Written communication only** — no calls required at any stage.

Korean · English · Chinese.
RWS TrainAI language assessment: Korean 35/35, English 34/35, both *Proficient User*.

Gyeonggi-do, South Korea · [jigonyoo.com](https://jigonyoo.com) · [dev.to/jigonyoo](https://dev.to/jigonyoo)
