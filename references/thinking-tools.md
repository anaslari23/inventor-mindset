# Thinking tools for invention

## Contents
1. Unsticking checklist
2. Inversion and pre-mortem
3. Contradiction thinking (TRIZ-lite)
4. Prior art check
5. Experiment design
6. Software-specific invention prompts

## 1. Unsticking checklist
When no good idea is appearing, work through these until one lands:
- Restate the problem as if explaining it to a smart 12-year-old. Where do you stumble? That is the hard part.
- Solve a smaller or simpler version first, then generalise.
- Solve the reverse problem (verify instead of generate, decode instead of encode).
- Remove the hardest requirement and see what becomes possible; then ask how to get it back cheaply.
- Look at the data. Print 20 real examples. Patterns that specs never mention show up here.
- Ask what would make the problem disappear instead of getting solved.

## 2. Inversion and pre-mortem
- **Inversion**: ask "How would I guarantee this fails?" then avoid those things. Often reveals the true critical path.
- **Pre-mortem**: assume it is six months later and the project failed. Write the three most likely reasons. Address the top one now.

## 3. Contradiction thinking (TRIZ-lite)
Great inventions often resolve a trade-off instead of accepting it.
- Name the contradiction: "I want X but improving it worsens Y" (faster vs. accurate, flexible vs. simple, private vs. useful).
- Resolve it by separating in **time** (precompute now, serve later), **space** (split hot and cold paths), **scale** (different rule per tier), or **condition** (different behaviour when input is easy vs. hard).
- Ask whether a hybrid keeps the benefit of both.

## 4. Prior art check
Before claiming something is new:
- Search for the idea under 3 different names (the field's term, the plain-English term, the adjacent field's term).
- Check papers, GitHub, and package registries.
- If similar work exists, state exactly what differs: the mechanism, the assumption it drops, or the case it handles better.
- Reusing good prior art is a win, not a failure. Inventing something that already exists wastes time.

## 5. Experiment design
- Write the hypothesis as a falsifiable sentence: "If this works, X will be at least N% faster / Y errors will drop to zero on dataset Z."
- Pick one metric and a baseline before running.
- Change one thing at a time.
- Keep the experiment under an hour of effort where possible.
- Record the result even when it is negative.

## 6. Software-specific invention prompts
- Can this be computed once instead of on every request?
- Can the data structure make the hard operation trivial (the right index, trie, graph, log, or CRDT)?
- Can the system learn from its own usage or failures?
- Can verification be cheaper than generation, and can that asymmetry be exploited?
- Can two components be merged so the interface between them disappears?
- Is there a constraint (schema, protocol, language) that could be turned into a feature?
- What would this look like with no UI, or with only a UI?
- If an LLM is involved: what part truly needs a model, and what part is better as deterministic code? Can the model be made to check, critique, or search instead of just generate?
