# How it works

At a high level, CogNarr reads a narrative and builds a structured representation of what it means, then lets a person refine that representation until it matches their intent:

- It reads the text and proposes a formal semantic structure for each sentence.
- Where a word, a reference, or an identity is uncertain, it keeps a set of candidates rather than forcing a decision.
- It resolves these interdependent decisions jointly, using the evidence each provides about the others.
- A person can inspect the result, correct it, rephrase the text if it helps the system to understand. Corrections will persist and be revisable.
- The resulting story graph can be queried for its argument structure, its timeline, the entities and their roles, and the consistency and entailment of its statements, and their modality. As well, information in the story graph can be viewed and edited in multiple presentations, each showing a unique aspect of narrative meaning. 

## Figures

```@raw html
<img src="/assets/fig1.png" alt="CogNarr architecture" width="530" style="border:1px solid #cbd0d8;border-radius:4px">
```

*Figure 1. Architecture. Narrative text, the lexicon, and external resources feed a parse-and-resolution engine that builds the story graph. Edits and corrections feed back into the engine, which reparses and resolves with each cycle.*

```@raw html
<div style="overflow-x:auto"><img src="/assets/fig2.png" alt="Resolution loops" style="width:1360px;max-width:none;border:1px solid #cbd0d8;border-radius:4px"></div>
```

*Figure 2. Resolution loops, inside the parse and resolve engine of Figure 1. Coreference forms an outer loop around an inner sense-and-identity loop, each iterating until a fixed point is reached. Corrections, timeline markup, and issues surfaced by querying enter as in Figure 1 and trigger a fresh reparse and resolve.*
