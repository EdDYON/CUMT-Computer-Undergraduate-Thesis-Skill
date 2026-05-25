---
name: cumt-thesis-writing
description: Use when analyzing, organizing, revising, or formatting a China University of Mining and Technology (中国矿业大学) computer-related undergraduate graduation design thesis / 本科毕业设计（论文） from real project materials, especially for template-first layout, project fact extraction, feature-sync writing, figure/table/equation/reference checks, WPS/Word docx handling, format-detection report fixes, marked-section naturalization / lowering template-like expression, and academic-integrity-safe thesis support.
---

# CUMT Computer Undergraduate Thesis

## Boundary First

This skill supports technical analysis, material organization, structure checking, conservative revision, and template layout for CUMT computer-related undergraduate graduation theses.

Do **not** use it as a ghostwriting, fabrication, plagiarism, paper-polishing, or academic-review-evasion tool. The final thesis content, claims, experiments, screenshots, references, and conclusions must be independently understood and verified by the student under advisor and school requirements.

When the user asks for a full thesis draft, first ground the work in real inputs. If a claim, function, dataset, screenshot, reference, or experiment cannot be verified from provided materials or project files, mark it as missing and ask for evidence instead of inventing it.

## Quick Start

1. Work from a copied template or copied thesis file. Never edit `assets/cumt-thesis-template.doc` in place.
2. Gather the highest-value inputs: school template, task book, proposal, sample thesis, thesis title, project code, database schema, screenshots, test notes, references, and advisor-specific requirements.
3. Read [references/template-spec.md](references/template-spec.md) when section order, caption rules, page numbering, bilingual contents, or CUMT template layout matter.
4. Read [references/project-first-workflow.md](references/project-first-workflow.md) when the thesis is based on a real software system, website, platform, database project, or engineering implementation.
5. Freeze a project fact base before drafting or revising. Use source code, database tables, screenshots, logs, and tests as evidence.
6. If the user mentions `格式检测`, `格式批注`, `维普格式检测`, `格式检查分析`, or similar reports, first parse the marked issues and fix only the marked scope unless the user explicitly requests a global format pass.
7. If the user mentions `降AI率`, `AI检测`, `疑似AI`, `模板化表达`, or similar wording, treat the task as integrity-preserving naturalization: improve specificity and readability, but do not claim or optimize for evading detection.
8. For WPS-only environments, keep formatting conservative: reuse existing styles, avoid aggressive restyling, update fields/contents through WPS when possible, and verify by exported PDF or rendered pages.
9. Report what was changed, what was only checked, what still needs human confirmation, and which claims lack evidence.

## Source Priority

Resolve conflicts in this order:

1. Formal school handbook, task book, advisor instruction, or live template requirement
2. The actual school template file being edited
3. User's explicit request for this document
4. Sample thesis structure and style
5. Real project source code, database schema, API routes, tests, screenshots, and logs
6. README, deployment notes, demo copy, or older design notes

Treat promotional copy, stale README descriptions, and unsupported "future" features as low-confidence. Do not write them as completed work unless the project files prove they exist.

## Working Modes

### Project Evidence Mapping

Use this before major writing or revision. Extract:

- thesis title and framing
- real user roles
- implemented modules
- frontend pages and backend endpoints
- database entities and key fields
- business flows
- algorithms, formulas, or rules actually used
- screenshots and diagram needs
- test evidence and known limitations

Keep a separate "needs user evidence" list for missing screenshots, references, data sources, and advisor-only requirements.

### Conservative Draft Support

Use only after the fact base is stable. Prefer grounded paragraphs, outline suggestions, table/figure descriptions, and revision guidance over unsupported full-body generation.

Write in a natural undergraduate thesis style: formal, specific, and plain. Reduce empty phrases such as "complete closed loop", "provide strong support", "significant improvement", and "important practical value" unless the text explains the concrete data path or test result behind the claim.

### Detection-Guided Naturalization

Use this when the user provides AI-detection highlights, suspicious-text marks, or asks to reduce template-like expression. Frame the work as readability, specificity, and fact-bound revision, not as bypassing a detector.

- Use the highlighted or named paragraphs as the default scope. Do not rewrite unmarked sections unless the user asks for a full-language pass.
- Preserve thesis title, chapter logic, data, table names, field names, model names, references, screenshots, and test conclusions.
- Keep revised paragraphs close to the original length, usually 80%-120%, unless the user asks for compression.
- Replace broad claims with concrete implementation facts: user action, page/component, API/service, database table/field, data flow, test step, observed limitation.
- Avoid unsupported evaluation words such as "significantly improves", "fully proves", "strongly supports", "important practical value", "complete closed loop", "empowers", and "production-ready".
- Add boundary wording when needed: "prototype", "demo data", "current implementation", "observed during testing", "requires manual review", or "not yet verified in long-term classroom use".
- For English abstracts, keep the meaning aligned with the Chinese abstract. Prefer natural, accurate wording over highly polished template phrases such as "To address this problem" or "The results show that".
- Produce a change explanation or diff that maps original wording to revised wording and lists remaining human-review items.

Load [references/project-first-workflow.md](references/project-first-workflow.md) for chapter-specific naturalization patterns.

### Template-First Layout

Use this when the user already has a draft and needs it placed into the CUMT template. Preserve cover pages, declarations, review forms, abstract pages, contents pages, section breaks, headers/footers, page numbering, and institutional styles.

Prefer in-place replacement and style reuse over rebuilding the document.

### Feature Sync

Use this when project code changes after the thesis draft already exists. Compare the changed files with the thesis, then update only the affected places:

- requirements and module tables
- implementation descriptions
- screenshots and captions
- database table descriptions
- test cases
- conclusion or limitation statements

Do not rewrite unrelated chapters.

### Final Format Audit

Use this near submission. Focus on format, numbering, layout, citations, and conservative language cleanup:

- figures, tables, algorithms, equations, captions, and body references
- heading hierarchy and numbering
- TOC and English contents
- page numbering, section breaks, and blank pages
- GB/T 7714 reference consistency
- placeholder text, unsupported claims, and over-polished template language

### Format-Detection Precision Fix

Use this when the user provides a format-check report, annotated `.docx`, or detected-error folder.

- First create an issue list with location, issue type, current problem, proposed fix, auto-fix safety, and human-confirmation need.
- Fix only issues that are marked in the report or directly caused by recent edits, unless the user explicitly requests a global cleanup.
- Keep the original file and create a clearly named copy such as `_格式标注精修版`, `_页码修正版`, or `_格式批注修订版`.
- Do not globally change fonts, spacing, headings, captions, page numbers, or references just because one instance is marked.
- When a comment concerns a reference, fill missing URL/access date/DOI only from verifiable material. If not verifiable, mark it for human completion instead of inventing metadata.
- Be careful with headers and page numbers. Do not add chapter-title fields into footers unless the template requires it; STYLEREF-style fields can make a page number area display text such as `1 绪论`.
- After fixes, generate an automatic modification list, human confirmation list, and high/medium/low priority rework list.

Load [references/template-spec.md](references/template-spec.md) for detailed report-driven formatting rules.

## Document Editing Rules

- For `.docx`, prefer `python-docx` for structured edits and WPS/Word COM only when fields, contents, pagination, export, or page numbering require the word processor.
- Always keep the original thesis file. Write a clearly named working copy such as `_修订版`, `_格式规范版`, or `_功能更新版`.
- For detection-guided tasks, name outputs by task and scope, for example `_标注段落自然化修订版`, `_格式标注精修版`, `_页码修正版`, plus a `.md` explanation or diff.
- After meaningful edits, verify that the document opens, headings still exist, image/table counts are reasonable, references remain readable, and exported PDF pagination is not obviously broken.
- If WPS cannot open a file, check for file locks or open WPS instances before assuming the docx is damaged.
- Do not leave temporary placeholder text such as "待补充", "这里插图", "TODO", or tool notes in the final thesis.
- Do not leave terms such as "降AI率", "AI痕迹", "检测", "改写策略", or tool workflow notes inside the thesis body.

## Figures, Tables, Equations, and References

- Figures need clear body references before placement. Captions go below figures and should be short, such as `图4-7 能力分析`; add the matching English caption when the template/sample uses bilingual captions.
- Avoid pages that contain only stacked images. If multiple screenshots must appear consecutively, add concise analysis below or between them.
- Use high-resolution real screenshots. If screenshots are blurry, ask the user for better captures or regenerate diagrams in a clean white-paper style.
- Tables need titles above the table. Use three-line table style when possible. Database design often benefits from both an E-R diagram and a core table description table.
- Equations should be inserted as real Word equations or stable equation objects when possible. Avoid plain-text formulas with broken underscores or ambiguous symbols. Number important formulas consistently.
- References must be real and relevant. Do not fabricate author names, titles, journals, years, DOI, URLs, volume/issue, or pages. If reference information is missing, mark it as missing.
- Check requirements such as total reference count and foreign-language reference count against the student's handbook or advisor instruction.
- When the user asks for cross-references, use Word/WPS fields where practical; otherwise keep captions and body references textually consistent and flag field updates for manual WPS verification.

## Academic Integrity Guardrails

- Never invent modules, data, screenshots, experiments, user counts, performance percentages, survey results, citations, or advisor feedback.
- Do not convert demo data into "large-scale real teaching data".
- Do not claim a prototype is a mature commercial system.
- Do not state that a model is significantly better unless the available experiment supports that exact conclusion.
- Do not optimize text for evading detection. It is acceptable to make writing clearer, more specific, and less template-like, but the goal must be accuracy and readability.
- When responding to "AI rate" requests, explicitly keep the goal on academic integrity, project specificity, and removal of template-like wording. Never guarantee a score or imply that detector results can be reliably controlled.
- AI-assisted features inside the student's project must be described according to their real boundary. For example, AI-generated questions usually remain candidate questions requiring teacher review.

## Resources

- `assets/cumt-thesis-template.doc`: bundled CUMT writing template asset. Copy before use.
- [references/template-spec.md](references/template-spec.md): CUMT template order and formatting notes.
- [references/project-first-workflow.md](references/project-first-workflow.md): project-based thesis evidence workflow, chapter rhythm, and final audit checklist.
