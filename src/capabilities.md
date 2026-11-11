# What CogNarr does

CogNarr reads a narrative and builds a story graph you can inspect and correct. The story view shows the narrative, the semantic graph built from the selected sentence, and an inspector for any element.

```@raw html
<img src="/assets/story-view.png" alt="The CogNarr story view: the narrative text, the semantic graph built from a sentence, and an inspector panel for the selected element." style="border:1px solid #cbd0d8;border-radius:4px">
```

- CogNarr transforms natural-language narrative into a formal, queryable semantic graph.
- It represents uncertainty explicitly, as soft distributions across the many dimensions of a reading, such as word sense, coreference, and entity identity.
- It captures a narrative's argument structure, its timeline, and the modality of its claims, including predictions and conditionals.
- It lets a writer inspect and correct the graph until it reflects their intended meaning, with corrections that persist yet remain revisable.
- It supports precise communication between software agents over a shared semantic structure.
