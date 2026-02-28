# Process Logs

A method for documenting how things are actually built — and learning from it.

---

## What is a process log?

A process log is a thinking tool. You write down what happened — the decisions, the surprises, the dead ends — and the act of writing forces you to understand what you actually did vs. what you think you did. When you revisit it later, you notice things you missed the first time. Patterns across entries. Contradictions between what you planned and what worked. Connections between ideas that seemed unrelated when you wrote them.

Writing the log makes you think. Revisiting the log makes you rethink. Over time, the accumulated entries reveal the shape of what you're building more clearly than any plan could.

---

## The entry pattern

Every entry follows this structure:

```markdown
## Entry N — [Title]

**Date:** [Date]
**Context:** [What triggered this entry — conversation, observation, research, experiment]

### [What happened / What was explored]

[Description]

### What this reveals

[Insights, patterns, connections to previous entries]

### What to explore next

[Questions or directions opened by this entry]
```

The "what this reveals" section is where the rethinking happens. It's easy to describe what you did. The harder part — and the part that produces the learning — is articulating what it means. What changed in your understanding. What assumption broke. What two things turned out to be the same problem.

---

## Numbering and continuity

Each process log file is sequentially numbered with a descriptive title:

```
00-origin.md
01-workflow-decision.md
02-reliability-evaluation.md
```

Entry numbers continue sequentially across files. Entry 1 might be in `00-origin.md`, Entry 5 in `01-workflow-decision.md`, Entry 6 in `02-reliability-evaluation.md`. This preserves the timeline even as the log grows across multiple files.

Each file starts with a reference to the previous one:

```markdown
# [Project] — Process Log #01 — [Title]

> Layer 3: Raw history.

**Previous:** Process Log #00 — [Title] (`00-origin.md`)
```

---

## Where it fits

The process log is one of three layers of documentation. They serve different purposes and should never collapse into one document:

| Layer | What it is | Tone |
|-------|-----------|------|
| **Spec** | Clean definition of what to build and how it's structured | Clear, reusable, no narrative |
| **Lesson** | Structured path someone follows to actually build it | Practical, direct |
| **Process Log** | What actually happened — raw, honest, time-stamped | Reflective, personal |

When they mix, all three suffer — the spec gets narrative-heavy, the lesson loses structure, and the process log gets sanitized. Keeping them apart means each one can do its job.

---

## How to use this

1. **Log as it happens.** The value is in capturing what you'd forget or sanitize if you waited.
2. **Write "what this reveals" every time.** That's the section that turns a record into a learning process.
3. **Revisit previous entries.** The process log is a feedback loop. Each revisit surfaces patterns and contradictions that weren't visible when you wrote the entries.
4. **Keep it honest.** The process log gets its value from being raw. The moment you start writing for an audience, it stops being useful as a thinking tool.

---

## Projects

Each directory is a real project with its own process log history.

| Project | What it is |
|---------|-----------|
| [thinking-tool/](thinking-tool/) | Exploring a tool that guides how to think — from seed observation through scientific grounding to design implications. The process of exploring the idea is itself a demonstration of what the tool would do. |

---

*Started: February 2026*
*Context: [Outcode Thinking](https://outcodethinking.com) — rethinking what it means to be a developer*
