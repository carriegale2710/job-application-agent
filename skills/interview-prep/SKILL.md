---
name: interview-prep
description: Prepare for an interview from an application's criteria, research and the story bank - likely questions with matched STAR stories, honest answers for gaps, company facts to know, and questions to ask. Use when the user gets an interview, or asks to practise for one.
---

# Interview prep

Input: `criteria.md`, `research.md`, the documents sent (`resume.md`, `cover-letter.md`, `selection-criteria.md`), `resume/stories.md`, and any interview details from the user.
Output: `applications/<company>-<role>/interview-prep.md`.

Ask once: "What do you know about the interview? Format, length, who is on the panel, any technical test?"

## Steps

1. **Likely questions.** For each vital criterion, write 1-2 behavioural questions ("Tell me about a time you...") and, for `can` criteria, 1 technical question. Add the usual openers: "Tell me about yourself", "Why this role?", "Why us?"
2. **Match a story.** For each question, pick the best story from `stories.md`. Use each story at most twice. If no story fits, run the gap interview (`master-resume`, `references/gap-interview.md`) and add the new story to `stories.md` first.
3. **Answer outlines.** Give each story as 4 short STAR lines, not a script. The user says it in their own words.
4. **Gaps.** For each `gap` in `criteria.md`, outline an honest answer: what they have that is closest, and how they would learn the rest. Never suggest claiming the skill.
5. **Know what you sent.** List every claim in the sent documents that the panel may probe, with the story behind it.
6. **Company facts.** Pick 5-6 facts from `research.md` to know cold, with their sources.
7. **Questions to ask.** Write 3-5 questions based on the research hooks. Do not ask anything the website answers, and do not ask about salary first.
8. **Technical topics.** For tech roles, list the tools and concepts in `criteria.md` keywords to revise, ordered by how often the ad mentions them.

## Format

```markdown
# Interview prep — <Role>, <Company>

## Interview details
- Date and time:
- Format: <phone | video | in person | panel | technical>
- Panel:

## Tell me about yourself
<4-5 lines: who you are, what you bring that matches the vital criteria, why this role>

## Likely questions
### <Criterion>
**Q:** <question>
**Story:** <story title from stories.md>
- S:
- T:
- A:
- R:

## Gaps and honest answers
| Criterion | What you have | How you would close it |
|---|---|---|

## Claims they may probe
| Claim (document) | Story behind it |
|---|---|

## Company facts to know
1. <fact> — <source>

## Questions to ask them
1.

## Technical topics to revise
```

## Rules

- Every story and claim must already exist in `resume/master-resume.md` or `resume/stories.md`.
- Answers are outlines. Do not write word-for-word scripts.
- Offer a practice round: ask one question at a time, then give feedback on structure (did it follow STAR, end with a result, and link back to the role).
