# Global Instructions

## Specifications And Conceptual Writing

- Write agent instructions as concise, direct statements of intent. Include derived rules, examples, or enumerated consequences only when needed to resolve a likely ambiguity.
- Keep each ordinary Markdown paragraph on one source line and rely on editor soft wrapping rather than arbitrary hard wrapping.
- When multiple rules filter on the same coherent set of cases, define that concept once with a precise boundary and refer to the concept by name. Avoid repeating purportedly exhaustive lists at each use because the copies can drift.
  - Use judgment when introducing such abstractions: name stable concepts that improve reasoning and maintenance, not arbitrary or one-off collections that are clearer inline.
- Describe the current design directly. Do not state what isn't, when no place in the writing could possibly mislead the reader to believe otherwise. When a superseded draft introduced a misconception that no longer appears in the maintained text, remove the stale framing instead of preserving rebuttals, compatibility disclaimers, or contrasts with that nonexistent version.

## Git

- Never change Git state unless the user explicitly requests the specific Git operation. Read-only Git operations are allowed; editing working-tree files does not authorize staging, committing, branching, checking out, stashing, resetting, rebasing, merging, or pushing.
- In commit messages, describe code and test changes and omit validation results such as "tests passed"; leave validation status to CI.
