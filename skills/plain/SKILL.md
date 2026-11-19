---
name: plain
description: Restate your previous answer, or text the user pastes, in clear everyday language for someone who is not a developer. Use when the user types $plain or @plain, asks for a plain-English version or a simpler explanation, or says they didn't understand.
---

# Plain

Rewrite your last answer, or the text the user gives you, for a reader who is smart but does not write code and did not watch the work happen. When they finish reading they should be able to say what happened, whether it is finished, and what they have to do.

How to write it:

- **Start with the answer.** One or two sentences giving the outcome or the main finding. If something is unfinished or not working, it goes here.
- **Explain by effect.** Describe each cause or finding by what a customer or the business would notice, with a small concrete example if the original has one. Skip where it sits in the code.
- **Say what is different now**, if anything changed, and the evidence that it works. If nothing was changed, as in a review, a diagnosis or an answer, say so in one sentence.
- **End with their next step.** Close with a line that begins "What you need to do:". Work it out; don't fill it in by habit.
  - If this is your own work from this conversation, you know more than your last message said. Check what is still true now: is anything unfinished or unchecked? Does anything need a decision, a password or another person? Did the problem leave damage behind that the fix does not repair, such as wrong records, earlier reports, or customers already affected? Each of those becomes a step or a decision for the reader.
  - If you are rewriting text somebody pasted, go only by what it says. If it does not say whether anything is needed, write "the report doesn't say", and name the one question worth asking.
  - Keep what they must do apart from what they may do: "Nothing is required. To see the corrected totals, run the report again."
  - If the original tells a developer how to fix something, turn that into a decision or request this reader can make, such as "ask for these three fixes before launch". Don't hand them instructions for doing the work.
  - Write "nothing" only after checking the first point and finding nothing.

Rules:

- Use only facts from the original and, when it is your own work, from what you did and saw in this conversation. Don't guess. Don't drop anything the reader would need: warnings, things not done, things not checked, numbers that show the size of a problem.
- Use everyday words: "automatic checks" for tests, "the product list" for a catalog, "New York time" for a time zone code. Assume the reader has never met words like token, endpoint, cache, sync, environment or API. If one has to stay, explain it in a few words the first time: "an access token, which works like a password".
- Leave out file names, function names, setting names, commands and code formatting unless the reader must type or pass along that exact text. If they must, say what it is and what to do with it.
- Write ordinary prose in short paragraphs. No section labels apart from the closing "What you need to do:" line. Use numbered points only when the original lists separate items.
- Aim for the length of the original. Never run more than half as long again. Where the original is already clear to this reader, keep its wording and change only what needs changing.
- Don't do any new work or change anything. This is a rewrite only.
