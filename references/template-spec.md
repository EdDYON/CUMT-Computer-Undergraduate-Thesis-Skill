# CUMT Thesis Template Spec

## Scope

- Source asset: `assets/cumt-thesis-template.doc`
- Source origin: 中国矿业大学毕业设计（论文）撰写模板
- File type: legacy Microsoft Word `.doc`
- Reliability rule: the live template file is authoritative. These notes guide editing but do not replace formal school or advisor requirements.

## Mandatory Section Order

The bundled template commonly includes these parts:

1. cover page / title page
2. originality statement
3. integrity commitment
4. authorization statement
5. acknowledgement
6. graduation design thesis task book
7. advisor review form
8. reviewer review form
9. defense and comprehensive score form
10. Chinese abstract
11. English Abstract
12. Chinese contents
13. English Contents
14. main body
15. references
16. foreign-language translation section, if required
17. appendix, if required

If the advisor or current handbook says a section is not required, follow that requirement and remove the section cleanly from the contents.

## Main Body Shape for Computer/System Theses

A practical structure is:

1. 绪论
2. 相关技术与理论基础
3. 系统需求分析与总体设计
4. 系统详细设计与实现
5. 系统测试与结果分析
6. 总结与展望

Adjust chapter names to match the task book, sample thesis, or advisor instruction.

## High-Confidence Formatting Rules

- Prefer in-place replacement over rebuilding pages manually.
- Preserve section breaks, headers/footers, page-number settings, review forms, and declaration pages.
- Chinese abstract heading is centered and bold; body generally uses Songti small-four with fixed line spacing close to 20 pt.
- English abstract heading is centered and bold; body generally uses Times New Roman small-four with similar line spacing.
- Keywords labels should follow the template's bolding and spacing.
- Main body Chinese text generally uses Songti small-four; English inline text generally uses Times New Roman.
- The contents usually list headings to level 2 unless the school or advisor requires deeper levels.
- Level-3 headings usually do not need English translation.
- Figure captions are below figures and centered.
- Table captions are above tables.
- When the template/sample uses bilingual captions, keep Chinese and English caption lines paired.
- Page numbering often uses Roman numerals for front matter and Arabic numerals for main text; verify with the current template and sample.

## Figure Rules

- Body text should introduce or explain a figure before the figure appears.
- Keep figure names short: `图3-2 学生学习闭环`, not long sentence-style captions.
- Prefer bilingual captions only when required by template/sample.
- Do not let a page become a stack of unrelated screenshots. Add analysis text or resize/move figures.
- Use clear screenshots; if printed text would be unreadable, ask for a better capture or recreate the diagram.
- For multi-panel figures, explain each subfigure in the body.
- Avoid splitting a figure and its caption across pages.

## Table Rules

- Table title goes above the table.
- Prefer three-line tables for formal thesis presentation.
- Keep table numbering chapter-based, such as `表3-1`, `表4-2`.
- Introduce and explain tables in the body.
- Avoid cramped tables and broken cross-page tables unless the template explicitly supports continued tables.
- Database chapters often benefit from a concise "core table description" table in addition to the E-R diagram.

## Equation and Algorithm Rules

- Use Word equation objects or stable equation formatting when possible.
- Avoid plain-text formulas that create garbled underscores or broken symbols.
- Number important formulas by chapter, such as `(4-1)`.
- Define formula variables immediately after the formula.
- Keep long code listings out of the main body. Use algorithm tables, pseudocode, or appendices for longer code.

## Contents and Field Rules

- If using Word/WPS automatic contents, update fields after heading changes.
- Check both Chinese contents and English Contents if both exist.
- If English Contents is generated manually or with fields, ensure it does not inherit wrong indentation or page numbers.
- After removing translation or appendix sections, remove their contents entries as well.

## Reference Rules

- Use GB/T 7714 style unless the school gives a different rule.
- Check reference type markers: `[J]`, `[C]`, `[D]`, `[M]`, `[EB/OL]`.
- Do not fabricate missing information. Mark unknown volume, issue, pages, DOI, or access date for human completion.
- Verify the total number of references and foreign-language references against the student's handbook or advisor instruction.

## WPS Practical Notes

- Many students only have WPS. Keep layout edits conservative and avoid operations that depend on Microsoft Word-only behavior.
- Use WPS to update fields, contents, and pagination when available.
- If WPS COM automation fails to open the file, check whether the document is already open or locked.
- Export to PDF for page-level review when possible.
- If no reliable renderer is available, perform structural checks with `python-docx` and clearly mark layout items that need manual review.
