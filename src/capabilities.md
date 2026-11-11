# What CogNarr does

CogNarr reads a narrative and builds a story graph you can inspect and correct. The semantic graph below is built from a short passage: each node is an entity or event carrying its word sense, and the labeled edges are the thematic roles and discourse relations that bind them.

```@raw html
<img src="/assets/sdrs.png" alt="A CogNarr semantic graph built from two clauses: entities and events labeled with their word senses, connected by thematic-role and discourse-relation edges." style="border:1px solid #cbd0d8;border-radius:4px">
```

*A semantic graph for two clauses, showing entities and events with their word senses, the thematic roles that connect them, and the discourse relation between the clauses.*

- CogNarr transforms natural-language narrative into a formal, queryable semantic graph.
- It represents uncertainty explicitly, as soft distributions across the many dimensions of a reading, such as word sense, coreference, and entity identity.
- It captures a narrative's argument structure, its timeline, and the modality of its claims, including predictions and conditionals.
- It lets a writer inspect and correct the graph until it reflects their intended meaning, with corrections that persist yet remain revisable.
- It supports precise communication between software agents over a shared semantic structure.
