<img src="assets/icon.svg" width="64" height="64" alt="">

# Chat-3P0

Three short skills that make GPT-6.2 Astra easier to work with in Codex.
Free, open source and tested in the open.

**Version 0.1, the first public version.** The skills work today. They are still being tested, and
which version ships next is decided by blind rankings that anyone can take part in.

**[Help decide what ships: rank four replies, about two minutes](https://livibesllc.com/chat3p0/rate/)**

## The skills

| Skill | What it does |
| --- | --- |
| [`$brief`](skills/brief/SKILL.md) | Say it roughly, get it done. Astra picks sensible defaults, finishes the job and tells you what it assumed. |
| [`$plain`](skills/plain/SKILL.md) | A report you can read. The same result, explained for someone who does not write code, ending with what you need to do. |
| [`$spark`](skills/spark/SKILL.md) | Fewer safe answers. For creative work, it pushes Astra away from its first idea. |

Each skill is one plain-text file. Read it before you use it: there is nothing hidden in any of them.

## Install

1. Download this repository (the green **Code** button, then **Download ZIP**) and unzip it.
2. Copy the three folders inside `skills/` into a folder named `.agents/skills/` in your own project,
   so that you have `.agents/skills/brief/SKILL.md` and so on.
3. Start Codex in that project.

## Use

Start your request with the skill's name:

```
$brief can you help make the report faster?
```

```
$spark Come up with a name and tagline for a new coffee shop.
```

Use `$plain` on its own, after Astra has finished and reported, to have that report rewritten for
someone who does not code.

## What testing has shown so far

Figures from this project's own runs of GPT-6.2 Astra in Codex CLI 0.169.1, November 2026.

- **A vague request no longer stalls.** Asked "I want customers to get a discount when they buy a
  lot", Astra on its own asked questions and changed nothing in 4 of 4 runs. With `$brief` it went
  ahead in 8 of 8.
- **Reports use fewer unexplained words.** On small tasks, readers playing a shop owner who does
  not code marked 8.9 unexplained words per report from Astra on its own and 2.8 with `$plain`.
- **Creative answers stopped repeating.** Across three creative prompts, five tries produced 4.0
  distinct ideas on average without `$spark` and 5.0 with it.

These are small tests on short tasks, scored mostly by AI readers. That is why the next step is
asking people.

## What has not been tested

- The ChatGPT desktop app, macOS and Linux. Every test so far ran in the Codex command-line tool on
  Windows.
- Jobs that run for hours.
- Models other than GPT-6.2 Astra.

## How a new version gets chosen

People rank replies without knowing where they came from. A new version of a skill ships when it is
ranked above the current one in at least 60% of head-to-heads, with at least 50 of them from 20
people, and only if it passes the project's accuracy checks.

The test requests, every reply, the scoring tools and the full results will be published here when
the current blind ranking closes. Publishing them sooner would show which reply came from where.

## Licence

[MIT](LICENSE). An independent project by LI Vibes LLC. Not affiliated with or endorsed by OpenAI
or Anthropic.
