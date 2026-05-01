# spark

Clarify vague ideas before planning — works with any AI, any platform.

Spark sits between *"I have a thought"* and *"I know what I want to build."* It assembles a virtual advisory team based on your idea's domain, then asks one question at a time until the idea is clear enough to hand off to planning.

## What it does

1. Detects the domain of your idea (software, business, creative, research)
2. Introduces a relevant advisory team in one sentence
3. Asks one key question at a time — no advice, no solutions, just questions
4. Outputs a three-line brief when the idea is clear
5. Hands off to your planning tool of choice

**Works in any language** — responds in whatever language you write in.

## Use it anywhere

**Claude Code (native skill):**
```bash
mkdir -p ~/.claude/skills/spark
cp SKILL.md ~/.claude/skills/spark/SKILL.md
```
Then trigger with `/spark` or say *"use spark to think through this idea."*

**Claude.ai / ChatGPT / Gemini / any other AI:**
Copy the contents of `SKILL.md` and paste it at the start of a conversation, or save it as a system prompt / custom instruction. The prompt works with any model.

**Any model via API:**
Use the contents of `SKILL.md` as your system prompt.

## Example

```
You:    I have an idea for an app that helps people capture ideas on their phone
Spark:  We're your product advisory team. First question:
        Is this solving your own problem, or one you've observed others having?
You:    My own — I keep losing ideas before I can write them down
Spark:  What's the simplest possible version of this?
...

[One-line definition] A zero-friction mobile capture tool for fleeting ideas,
                      for people who lose thoughts before opening a notes app
[Biggest unknown]     Whether users will stick with a dedicated app when
                      Claude/ChatGPT already do this
[Minimum next step]   Set up an Action Button shortcut on iPhone that opens
                      Claude voice input directly
```

## When to use

- You have a fuzzy notion and don't know what to do with it
- You want to think something through before committing to a plan
- You keep saying "I have an idea" but never do anything with it

**Not for:** ideas already clear enough to spec, debugging, or implementation work.

## License

MIT
