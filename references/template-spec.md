# CUMT Thesis Template Spec

## Scope

- Source asset: `assets/cumt-thesis-template.doc`
- Source origin: 中国矿业大学毕业设计（论文）撰写模板
- File type: legacy Microsoft Word `.doc`
- Reliability rule: the bundled template file is authoritative. The notes below were recovered from automated extraction and are intended to guide editing, not replace the template itself.

## Mandatory Section Order

1. 封面 / 扉页
2. 原创性声明
3. 诚信承诺书
4. 使用授权声明
5. 致谢
6. 本科毕业设计（论文）任务书
7. 指导教师评阅书
8. 评阅教师评阅书
9. 答辩及综合成绩表
10. 中文摘要
11. 英文 `Abstract`
12. 中文目录
13. 英文 `Contents`
14. 正文
15. 参考文献
16. 外文翻译部分
17. 附录

## Structural Notes

- The sample thesis topic inside the template is flotation research. Treat it as placeholder content and replace it completely.
- The template includes both Chinese and English contents pages.
- The extracted text shows Chinese abstract and English abstract sections with separate keywords lines.
- The extracted text shows a translation section split into `英文原文` and `中文译文`.
- The appendix section can contain code, procedures, or supporting material.

## Suggested Main-Body Shape for Software or System Theses

When the user's thesis is based on a software, website, management system, database platform, or similar engineering project, a practical main-body structure is:

1. 绪论
2. 需求分析 / 相关技术与可行性分析
3. 系统总体设计
4. 系统详细设计与实现
5. 系统测试 / 部署与验证
6. 结论与展望

Adjust the names to match the task book, sample thesis, or school wording. Prefer the template and the task book over any generic chapter names.

## Recovered Formatting Rules

### High Confidence

- Prefer in-place replacement over manual restyling.
- Chinese abstract heading is centered and bold, approximately small-second size; the `关键词` label is bolded.
- Chinese abstract body uses Songti small-four with fixed 20 pt line spacing.
- English `Abstract` heading is centered and bold, approximately small-second size.
- English abstract body uses Times New Roman small-four with fixed 20 pt line spacing.
- The `Keywords` label is bolded.
- Main body text uses Songti small-four; English inline text uses Times New Roman small-four.
- Main body line spacing is fixed at about 20 pt.
- The table of contents only needs to list headings down to level 2.
- Level-3 headings do not need English translation.
- Figure captions are placed below the figure and centered.
- Figure and table captions use paired Chinese and English caption lines that should follow the existing template style.

### Medium Confidence

- Front-matter declaration pages use bold centered headings with body text in KaiTi small-four and fixed 20 pt line spacing.
- Recovered annotations suggest Chinese chapter headings use bold HeiTi styles and paired English headings use bold Times New Roman styles.
- Recovered annotations also suggest:
  - primary headings use a larger bold style with single line spacing and about 0.5-line space before
  - second-level headings use a smaller bold style with about 0.5-line space before and after
  - third-level headings use a smaller HeiTi style
- Some cover-page title and metadata font notes were only partially recoverable. Reuse the live styles from the template instead of rebuilding the cover page manually.

## Practical Editing Rules

- Duplicate nearby styled paragraphs when adding a new heading, figure caption, or table caption.
- Refresh both contents pages after heading changes.
- Keep signature blocks, date fields, and review forms intact unless the user explicitly wants a simplified draft.
- If the user asks for a `.docx` version, convert a copied working file. Never overwrite the asset copy in this skill.
- If the user only has WPS, avoid aggressive restyling. Preserve existing paragraph styles and section breaks whenever possible.
