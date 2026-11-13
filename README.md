# concise

A plain-Markdown instruction file that makes an AI assistant answer in as many sentences as the answer has core points, with no openers, closers or filler. It works with any chat model or coding agent that accepts written instructions.

## Use it

**As a system prompt or custom instructions.** Copy everything in [`SKILL.md`](SKILL.md) below the `---` frontmatter block into your model's system prompt, custom instructions or project rules file.

**As a skill.** Agents that load `SKILL.md` skills can use the folder as it is. Clone it into the agent's skills directory:

```bash
git clone https://github.com/fzizzle/concise <your-agent's-skills-directory>/concise
```

Then ask for concise answers, or type `/concise` if your agent supports slash commands.

Say "stop concise" to turn it off.

## Example

> why does ice float?

Water molecules lock into an open hexagonal lattice when they freeze, which holds them farther apart than in the liquid. Ice is therefore about 9% less dense than water, so it floats.

## What it tells the model

1. Reduce the answer to its core points: those the user can't act without.
2. Order them, answer first.
3. Write each point once, plainly.
4. Stop after the last point.

It also lists what counts as core (mechanisms, risks of losing data or money, the one fact that would change the answer) and the wording habits to cut (praise openers, stacked hedges, inflated words, contrast frames).
