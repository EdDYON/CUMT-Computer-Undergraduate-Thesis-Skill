# Project-First Workflow

## Scope

Use this reference when the thesis is based on a real software, website, platform, management system, database project, or other implementation-heavy graduation project.

Do not use these defaults rigidly for theoretical, experimental, or purely literature-review theses. In those cases, keep the school template rules but relax the software-specific chapter and screenshot expectations.

## Minimum Useful Inputs

Prioritize these inputs when available:

1. school template
2. task book or proposal
3. sample thesis
4. thesis title
5. target word count or page target
6. project repo
7. README and project docs
8. database schema, API docs, test notes, screenshots, or deployment notes

If the user cannot provide all of them, continue with the strongest available set and state the missing pieces as assumptions.

## Intake Output

Before drafting long sections, summarize:

- which files and inputs are being used
- which sources are missing
- the proposed chapter outline
- target word count by chapter
- style or structure conflicts
- the planned working file name

If the user later adds a new template, sample, or task book, refresh this summary before continuing.

## Fact Base

Build a fixed project fact base before expanding prose. Capture at least:

- project objective
- target users or roles
- core modules
- main workflows
- major tables or entities
- key rules and constraints
- technology stack
- implemented features
- known limitations
- available evidence such as screenshots, logs, tests, or demo pages

Use this fact base as the source of truth for later chapter writing.

## Recommended Chapter Rhythm for Software Theses

### Chapter 1

- background
- research or project significance
- current status or related work if needed
- thesis structure

### Chapter 2

- requirements analysis
- feasibility
- development environment
- key supporting technologies

### Chapter 3

- overall architecture
- functional module breakdown
- role design or permission design
- key business flows
- database design

### Chapter 4

- make this the longest or near-longest chapter
- organize by major module
- for each major module, prefer:
  - module purpose
  - business flow or interaction logic
  - brief code or SQL evidence
  - real screenshot

### Chapter 5

- testing environment
- test cases
- execution results
- result analysis

### Chapter 6

- conclusion
- limitations
- future work

## Diagram, Screenshot, and Code Expectations

For software or web-system theses, the following usually provide the strongest evidence:

- system architecture diagram
- module structure diagram
- one or more key process diagrams
- E-R diagram or equivalent data-model view
- data tables where needed
- test-case tables
- real screenshots from major modules
- short code or SQL fragments that explain business rules

Keep large code listings out of the main body. Put them in the appendix if needed.

If the database design is large, split the E-R presentation into:

1. overall E-R view
2. one or more core-domain E-R views

## Reference Workflow

Use only real and relevant references.

Recommended sequence:

1. build a candidate pool
2. remove anything unverified
3. keep only sources that support the actual topic
4. format the final list consistently
5. check that the thesis body does not cite sources that are missing from the final list

Prefer recent sources unless the user or topic clearly requires older classics.

## Writing Guardrails

- Prefer concrete facts over empty praise.
- Do not invent modules, roles, tables, or test results that are not supported by code or project materials.
- Keep terminology consistent across chapters.
- Reuse real names from the project when they are suitable for an academic thesis.
- Avoid obvious AI filler such as repeated claims of "important significance", "good effect", or "high practical value" without evidence.

## Final Review Checklist

Before delivery, verify:

- the outline matches the confirmed plan
- the implementation chapter is substantial enough
- major modules in the implementation chapter have evidence
- screenshots are real and correctly titled
- diagram references match the actual diagrams
- chapter word counts are not wildly unbalanced
- placeholders are removed
- references are consistent and real
- appendix material is separated from the main body
- the final content still fits the CUMT template order
