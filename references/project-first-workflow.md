# Project-First Workflow

## Scope

Use this reference when the thesis is based on a real software system, website, learning platform, management system, database application, data-analysis project, or similar engineering implementation.

For theoretical or literature-review theses, keep the CUMT template rules but relax the software-specific screenshot, database, API, and test-case expectations.

## Minimum Useful Inputs

Prioritize these inputs:

1. school template, task book, proposal, or advisor notes
2. sample thesis or department formatting example
3. thesis title and expected page/word target
4. project source code and commit/change notes
5. database schema, migrations, seed data, or table screenshots
6. API routes, service-layer code, frontend pages, and route configuration
7. real screenshots, diagrams, test notes, logs, and exported charts
8. verified references and handbook requirements for reference count

If inputs are incomplete, continue with the strongest available evidence and keep a clear missing-material list.

## Fact Base

Before drafting or revising thesis text, build a fact base with these fields:

- project objective and application scenario
- target users and roles
- implemented modules and pages
- backend endpoints and service responsibilities
- database tables, key fields, and relationships
- data flow from user operation to persistence and analysis
- algorithms, rules, formulas, or model comparisons
- test environment and test cases
- screenshots, generated diagrams, and chart sources
- known limitations and prototype boundaries

Use this fact base as the source of truth for every chapter. When the project changes, update the fact base first, then sync only the affected thesis sections.

## Evidence Ledger

For each important claim, keep a simple ledger:

- Claim: what the thesis says
- Evidence: code file, table, screenshot, test record, or reference
- Thesis location: chapter/table/figure/paragraph
- Status: verified, partially verified, needs user material, or remove

This prevents the thesis from drifting into unsupported claims.

## Recommended Chapter Rhythm for Software Theses

### Chapter 1: Introduction

Ground the background in the course or application problem. Avoid generic "digital education is important" openings unless the paragraph quickly connects to the actual project.

### Chapter 2: Related Technology and Theory

Do not write pure textbook summaries. Connect each technology or theory to the implementation:

- Vue, Vite, Element Plus, ECharts, CodeMirror: frontend pages, forms, charts, SQL editor, or visualization
- FastAPI, SQLAlchemy, MySQL: endpoint routing, service layer, ORM tables, persistence
- Q matrix, knowledge tracing, cognitive diagnosis, recommendation: the actual tables, fields, or data flow used
- DINA/IRT/model comparisons: baseline or comparison roles, not exaggerated production claims

### Chapter 3: Requirements and Overall Design

Use functional tables, role paths, business flows, architecture diagrams, and database design. For database projects, include:

- E-R diagram or equivalent entity relationship view
- core database table description table
- mapping tables such as question-knowledge relations when they affect algorithms

### Chapter 4: Detailed Design and Implementation

Usually this should be the most concrete chapter. For each major module:

- module purpose
- page/component responsibilities
- backend route/service/data-table relationship
- key interaction flow
- real screenshot or diagram
- short code, SQL, pseudocode, or formula only when it explains the mechanism

Avoid long code screenshots. Use pseudocode, formulas, or a compact table if code would damage layout.

### Chapter 5: Testing and Result Analysis

Write what was actually verified:

- functional tests
- data-link tests from UI operation to database record to analysis result
- model comparison or algorithm checks
- abnormal-data handling if implemented
- performance or compatibility tests only when real test evidence exists

For prototype systems, say "supports prototype verification" rather than "proves teaching effectiveness".

### Chapter 6: Conclusion and Future Work

Summarize completed work, verified data links, and real limitations. Future work should be concrete:

- expand the question bank and real answer data
- improve Q-matrix annotation quality
- refine SQL error-type analysis
- improve teacher intervention suggestions
- add quality review for AI-assisted generated questions
- validate the system in longer real classroom use

## Syncing New Project Changes Into the Thesis

When the user reports new features or changed files:

1. Inspect the mentioned code files and routes.
2. Identify which thesis chapters are affected.
3. Update module tables, requirements, implementation text, screenshots, captions, and tests.
4. If the feature adds a new page, add or replace a screenshot only when the user provides a clear image or the app can be run and captured.
5. Add a test case for the new feature if it is user-facing.
6. Update conclusion only if the change affects completed work.
7. Do not inflate the feature beyond what the code implements.

## Figures and Diagrams

Strong software-thesis evidence often includes:

- system architecture diagram
- core business flow
- student/user workflow
- teacher/admin intervention workflow
- E-R diagram
- core database table description
- Q matrix or mapping-table illustration
- profile/diagnosis/recommendation process diagram
- model comparison chart
- real screenshots of major pages

Prefer clean white-background diagrams with consistent typography. Diagram names should be short and stable, such as "系统总体架构", "数据库实体关系", "能力分析", and "教师干预流程".

## Tables

Useful table types:

- functional module division
- core database table description
- field mapping table for key relationships
- algorithm variable explanation
- test environment
- functional test cases
- data-link and model experiment test cases
- reference candidate tracking when references are still being collected

Use tables to reduce repetitive prose. Keep captions short and place them according to the template.

## Data, Experiments, and Charts

- Use real test data, provided demo data, or explicitly labeled prototype data.
- Do not claim demo data is large-scale classroom evidence.
- If generated data is used only to test UI or pipeline behavior, label it as simulated or demonstration data.
- Use charts to explain system behavior or algorithm comparison, not to create unsupported effectiveness claims.
- When sample size or response matrix density is weak, say so plainly.

## Writing Style

Aim for a formal but natural undergraduate thesis style:

- Prefer specific data paths over empty evaluation language.
- Replace "the platform forms a complete closed loop" with the actual path, such as answer record -> knowledge mapping -> mastery snapshot -> student feedback and teacher analysis.
- Keep repeated terms consistent, but avoid starting many consecutive sentences with "the system", "the platform", or "this thesis".
- Reduce repeated chapter summaries that say the same thing as the chapter opening.
- Make limitations concrete and believable.

Improving clarity and reducing template-like wording is allowed. Do not rewrite with the purpose of evading detection or hiding authorship.

## Final Review Checklist

Before delivery, verify:

- original file is preserved and the output file has a clear new name
- headings and numbering still match the intended outline
- Chinese and English abstracts are consistent
- contents pages update correctly if they are field-based
- figure/table/equation numbering is continuous
- body references appear before major figures and tables
- screenshots are legible and not stacked without explanation
- formulas are not garbled
- references are real, formatted consistently, and cited in the body
- no placeholder text remains
- no unsupported function, data, experiment, or result has been added
- WPS/Word can open the file and exported PDF pagination looks reasonable
