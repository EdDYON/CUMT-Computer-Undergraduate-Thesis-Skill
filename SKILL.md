---
name: cumt-thesis-writing
description: Use when drafting, revising, or formatting a China University of Mining and Technology (中国矿业大学) undergraduate graduation thesis / 毕业设计（论文）, especially when the user wants to write from a real software or system project, combine project code with 开题报告/任务书/往届样文, and then fit the result into the saved school template for cover pages, declarations, abstracts, contents, main chapters, references, translation section, and appendices.
---

# CUMT Thesis Writing

## Quick Start

1. Gather as many of these as possible before writing: school template, task book or proposal, sample thesis, cover-page fields, word-count target, and project code or project documents.
2. Copy `assets/cumt-thesis-template.doc` to a working location before editing. Never edit the asset in place.
3. Preserve the existing styles, page breaks, and institutional forms in the copied template.
4. Read [references/template-spec.md](references/template-spec.md) for the school-specific section order and formatting notes.
5. Read [references/project-first-workflow.md](references/project-first-workflow.md) when the thesis is based on a real software, website, system, database, or engineering project.
6. If the user only has WPS, keep the layout edits conservative and use the template as-is; if Word becomes available later, use it for final pagination and field checks.

## Source Priority

Resolve conflicts in this order:

1. School template
2. Task book / proposal / formal school requirements
3. User's explicit request
4. Sample thesis
5. Project source code and database schema
6. README
7. Old deployment notes, demo copy, or legacy descriptions

Treat old introductions, promotional copy, and stale documentation as low-confidence sources unless the user explicitly asks to reuse them.

## Working Modes

### Template-First Formatting

- Use this when the user already has most of the thesis text and mainly needs it placed into the China University of Mining and Technology template.
- Preserve the template's structure, declarations, bilingual abstract pages, bilingual contents pages, translation section, and appendix placement.

### Project-First Drafting

- Use this when the user has a real project repo or project documents and wants to generate a thesis draft from those materials.
- Freeze project facts first, then map those facts into a thesis outline, then place the result into the school template.

### Final Cleanup

- Use this when the draft already exists and the remaining work is checking headings, figure and table captions, references, page order, and placeholder cleanup.

## Workflow

### 1. Intake Before Writing

- On the first thesis-writing request, prefer collecting missing materials before writing the full main body.
- Ask for the highest-value missing items first: template or sample thesis, task book or proposal, title, word-count target, and project repo or project docs.
- If the user explicitly says there are no more materials, continue with the available inputs and state the assumptions.
- Accept local file paths directly.

### 2. Freeze Project Facts

When the thesis is based on a real project, build a stable fact base before expanding prose. Capture at least:

- thesis title and target framing
- problem domain and project objective
- user roles
- core modules
- key business flows
- key entities or tables
- technology stack
- implemented features versus planned features
- testing evidence, screenshots, and deployable pages if available

Later chapters should expand from this fact base instead of re-inventing details chapter by chapter.

### 3. Analyze Template and Samples

- If the user provides a sample thesis or school template, analyze structure, word rhythm, heading depth, abstract style, keyword style, figure captions, table captions, and reference formatting before drafting the main body.
- If the recovered notes and the live template disagree, trust the live template asset.
- If a new sample thesis or new task book appears midstream, re-check the outline before continuing.

### 4. Confirm Outline and Word Budget

Before writing large sections, prepare a concise design package that includes:

- the input materials being used
- the proposed chapter outline
- target word count by chapter
- style notes and conflict items
- file naming plan

For software or system theses, the main body usually works best when `系统详细设计与实现` or the equivalent implementation chapter is the longest chapter.

### 5. Draft by Chapter

- Stay close to the word budget instead of inflating the thesis.
- Prefer project facts and concrete implementation details over empty evaluation language.
- Keep the tone similar to an undergraduate thesis sample, but avoid obvious template phrases and generic praise.
- Reuse the user's real module names, table names, business rules, and screen names where appropriate.

For software or system theses, use the patterns in [references/project-first-workflow.md](references/project-first-workflow.md):

- design chapter: architecture, module structure, key flows, database design
- implementation chapter: module purpose, key logic, screenshot, brief code or SQL evidence
- testing chapter: environment, cases, results, analysis

### 6. Keep Figures, Tables, Screenshots, and Code Grounded

- Do not add diagrams just to fill space; make them correspond to real modules or real workflows.
- Database design should include an E-R view when the project actually has a meaningful data model.
- If a full E-R diagram is too crowded, split it into a full overview and one or more core-domain diagrams.
- For software or web projects, each major module in the implementation chapter should usually include at least one real screenshot and one brief implementation snippet or SQL fragment.
- Put large code blocks into the appendix instead of the main body.

### 7. Fit the Draft into the CUMT Template

- Replace sample content in place instead of rebuilding the whole document from scratch.
- Update title, author, advisor, college, major, student number, and date directly inside the copied template.
- Keep the mandatory section order from [references/template-spec.md](references/template-spec.md).
- Maintain bilingual elements where the template uses them: title or labels, abstract pages, keywords, contents pages, and caption pairs.
- Keep the table of contents limited to level-2 headings unless the user asks for a deeper TOC.
- Do not translate level-3 headings into English.

### 8. Final Checks

Before delivery, check at least:

- mandatory sections are present and in the right order
- the chapter structure matches the chosen outline
- word count is near the target range
- headings, figure captions, and table captions are consistent
- references are real and relevant
- screenshots and diagrams are not placeholders
- appendix content is separated from main-body content
- the copied working file, not the skill asset, is being edited
- WPS pagination, contents fields, and page numbering still look reasonable

## Resources

- Use `assets/cumt-thesis-template.doc` as the exact template to copy from.
- Use [references/template-spec.md](references/template-spec.md) for the recovered section order and formatting notes.
- Use [references/project-first-workflow.md](references/project-first-workflow.md) for project-driven drafting rules, software-thesis chapter patterns, evidence expectations, and final review checklists.
