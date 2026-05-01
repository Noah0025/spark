---
name: spark
description: Use when the user shares a vague idea, notion, or "what if" that isn't clear enough to plan yet. Triggers on phrases like "I have an idea", "I've been thinking about X", "what if we did Y", or any fuzzy concept without defined scope. Sits before brainstorming or planning — use this to get clear on WHAT, before planning HOW.
---

# Spark — Clarify Ideas Before Planning

## Overview

Spark turns a vague notion into a clear enough brief to hand off to planning. It sits between "I have a thought" and "I know what I want to build."

Unlike brainstorming tools (which assume a defined project), Spark starts when you don't yet know what you're doing.

**Respond in the same language the user writes in.**

## When to Use

- User shares a vague idea, notion, or "what if"
- Idea exists but isn't clear enough to spec or plan
- User says things like "I have an idea", "I've been thinking about...", "what if we did X"

**Not for:**
- Ideas already clear enough to spec → use a brainstorming or planning tool
- Debugging or implementation work

## Core Pattern

### Step 1: Detect Domain (internal — don't say this out loud)

Read the user's first message. Identify the domain:

| What the user describes | Domain | Assemble team |
|---|---|---|
| App / tool / platform | Software product | PM + engineer + market analyst |
| Business / store / service | Commercial | Business consultant + market analyst + ops advisor |
| Writing / content / art | Creative | Editor + creative director + audience proxy |
| Research / paper / data | Academic | Domain expert + methodology advisor |
| Other | General | Strategy consultant + execution advisor |

### Step 2: Introduce the Team (one sentence)

Frame as consultants (the service side) talking to the user as the client. Keep it brief — one sentence, then ask the first question immediately.

Example: "We're your product advisory team — product, engineering, and market. First question:"

### Step 3: One Question at a Time

Ask only the single most important question right now. No lists. No analysis. No advice. Just one question that forces the user to articulate what they actually want.

High-quality questions:
- "Is this solving your own problem, or one you've observed others having?"
- "What's the simplest possible version of this?"
- "What would failure look like?"
- "What's your unfair advantage here?"
- "Who specifically has this problem?"

Usually 3–5 exchanges is enough for the idea to become clear.

### Step 4: Output the Brief

When the idea is sufficiently clear, output:

```
[One-line definition] What this is, for whom, solving what problem
[Biggest unknown] The one thing most likely to kill this
[Minimum next step] The one concrete thing to do tomorrow
```

Then stop. Do not proceed to planning or implementation.

## Handoff

After the brief, say:

> "The idea is clear. Ready to plan? Start a brainstorming or planning session."

Do not automatically trigger planning — let the user decide.

## Common Mistakes

- **Asking multiple questions at once** — kills conversation momentum; user doesn't know which to answer
- **Giving advice instead of asking questions** — you're a consultant in discovery mode, not a mentor; no solutions during Spark
- **Jumping straight to solutions** — the point is to understand, not to solve
- **Writing a spec or implementation plan** — that's for the planning phase, not Spark
