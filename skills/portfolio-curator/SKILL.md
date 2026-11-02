---
name: portfolio-curator
description: Shortlist the 2-4 portfolio case studies that best prove a role's criteria, with links and one-line mentions for the resume and cover letter. Use for design, front-end and other roles where a portfolio matters.
---

# Portfolio curator

Inputs: `criteria.md`, `research.md`, `resume/portfolio-index.md`.
Output: `applications/<company>-<role>/portfolio.md`.

## Build the index once

If `resume/portfolio-index.md` does not exist:
1. Get the portfolio URL from `resume/master-resume.md`, or ask the user.
2. Fetch the site and list each case study: title, link, one-line summary, skills and tools shown, outcome.
3. If the site cannot be fetched, ask the user to list their case studies.

Reuse the index for every later application. Update it when the user adds work.

## Shortlist for each application

1. Score each case study against the vital criteria in `criteria.md`, and against the company's products, domain and stack from `research.md`.
2. Pick 2-4 high-impact pieces. Fewer strong pieces beat many weak ones.
3. Show range only when the ad asks for breadth.

## Format

```markdown
# Portfolio shortlist — <Role>, <Company>

| Rank | Case study | Link | Criteria it proves | Why it fits this company |
|---|---|---|---|---|

## Resume mention
<one line for the contact block, profile or Projects subline>

## Cover letter mention
<one sentence for a middle paragraph, naming the top case study>
```

## Rules

- Never describe work that is not in the portfolio index or master resume.
- Select by criteria and research, not by what the user likes best.
- If the site lets the user reorder or pin work, suggest which piece to put first for this application.
