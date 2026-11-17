---
name: socratic-prd
description: Interrogate a product or project request Socratically until its real outcome, achievable success metric, and request-to-outcome fit are explicit. Use for PRD discovery, feature requests, project briefs, and requests whose proposed output may be mistaken for the underlying goal.
---

# Socratic PRD

Turn a proposed output into a decision-ready request by discovering its **destiny**: the outcome it must cause and the observable proof that the outcome occurred.

## Conduct the interview

Ask one focused question at a time. Make each question depend on the previous answer; prefer a short question with a concrete contrast over a questionnaire. Be relentless about unresolved reasoning, not repetitive or hostile.

Start from what is **certain now**: directly observed facts, supplied evidence, constraints, or explicit binding decisions. Briefly reflect the relevant certainty before asking what follows from it. Progressively expose assumptions by asking:

1. What situation exists now, for whom, and what evidence establishes it?
2. What change is actually wanted? Separate the proposed deliverable from the human or business outcome.
3. Why does that change matter, and what downstream end would make it valuable? Repeat “what would that achieve?” until the answer is an outcome rather than another artifact or activity.
4. Why should this request cause that outcome? Test the causal link, alternatives, counterexamples, dependencies, and failure modes.
5. What observable evidence would distinguish success from failure?

Challenge vague terms such as *better*, *engagement*, *useful*, *visibility*, or *adoption*. Turn them into an operational measure with, where relevant: population, behavior or quantity, baseline, target or threshold, timeframe, data source, and measurement owner. A metric is ready only when it is achievable, falsifiable, and practically verifiable. Do not invent missing values; ask for them or help the user choose a defensible value.

Keep a lightweight internal ledger of:

- certain facts and binding decisions;
- assumptions and their current certainty;
- candidate destiny;
- proposed result/request;
- success proof;
- unresolved contradictions or dependencies.

Use the ledger to avoid asking answered questions and to revisit answers that conflict.

## Completion gate

Finish only when all of these are explicit and mutually consistent:

- the request names the result to be produced;
- the destiny names the outcome for a defined beneficiary;
- the proof contains at least one achievable, falsifiable measure and a practical way and time to observe it;
- the causal link from result to destiny has been examined against meaningful alternatives and dependencies;
- the user has confirmed the distilled request, destiny, and proof.

There is no target number of questions. If the user chooses to stop before the gate is met, provide a clearly labeled **interim discovery summary** with open questions; never call it interview-complete.

## Evaluate only request-to-destiny fit

Judge the proposition: **“The requested result will achieve the clarified destiny, as demonstrated by the stated proof.”** Do not score novelty, effort, popularity, general product quality, or whether the request serves a different destiny.

This relativity is the governing principle: dancing can fully satisfy the destiny *moving the body* while weakly satisfying *getting a girlfriend*. Changing the destiny changes the evaluation even when the proposed result is identical.

Assign an integer fit score:

- **9–10:** the result directly and sufficiently produces the destiny under the stated conditions;
- **7–8:** strong fit with limited dependencies or residual gaps;
- **4–6:** partial or indirect fit; important assumptions remain;
- **1–3:** weak fit; the result mainly serves another destiny;
- **0:** no defensible causal fit.

Then label the epistemic support for that same proposition:

- **Certain** — directly evidenced fact or explicit binding decision. Use for causal fit only when evidence or logic establishes it, not merely because the destiny was explicitly chosen.
- **Probable** — best-supported conclusion, with meaningful evidence but residual doubt.
- **Plausible** — coherent hypothesis with insufficient evidence to prefer it.
- **Possible** — conceivable option or explanation not yet ruled out.

The score measures strength of fit; the label measures confidence in that judgment. State material conditions in the rationale rather than inflating either assessment.

Map the certainty label to a roadmap verdict:

- **Certain → Free to move**
- **Probable → Solid choice**
- **Plausible → Good bet**
- **Possible → No go**

Use the verdict determined by certainty even when the numeric fit score is high. A strong theoretical fit with little evidence can still be a no-go.

## Match the conversation language

Write the entire final output in the language used by the user during the interview. Translate the structural labels, certainty level, verdict, and dynamic headings into natural equivalents; do not leave English headings in an otherwise non-English result. Preserve the meaning of the four canonical certainty levels when translating them.

## Final output

After the user confirms the distilled formulation, use this compact structure:

```markdown
---

*{Interview finished}: {score}/10, {localized certainty level}. {localized verdict}.*

**{Request}:** {specific result to produce}

**{Destiny}:** {observable outcome for the beneficiary}

**{How it's proved}:** {baseline if relevant; target/threshold; population; timeframe; data source or verification method}

**{Why [localized certainty level]}:** {one or two sentences explaining the evidence and reasoning that justify this certainty level, including the decisive dependency or residual doubt}

**{What needs to change to move to [localized next level]}:** {the smallest concrete evidence, test, decision, or scope change needed to justify the next certainty level}

---
```

Choose the next level dynamically: Possible → Plausible, Plausible → Probable, and Probable → Certain. For Certain, replace the next-level heading and body with the localized equivalent of **“What needs to change: Nothing. Free to go.”**

A low score or no-go verdict is a valid finished result: it means discovery clarified that the proposed result poorly serves the chosen destiny or lacks adequate support, not that the interview failed.
