# 天津大学硕士论文写作技能

`tju-master-thesis` 是用于 Codex 的硕士论文写作技能，支持天津大学学术硕士和专业硕士论文的提纲设计、章节撰写、润色、中英文摘要、引用整理、Word/LaTeX 排版和格式审查。

依据为用户提供的《天津大学关于博士、硕士学位论文统一格式的规定（2021年修订202611更新扉页版）》。本仓库保留原始文件，未核验该版本为学校现行最新版；学院或学校另有适用要求时，应核对后采用。

技能区分原文要求、原文建议和写作建议，并记录新版扉页英文题目位置等歧义。写作以提供的研究材料为依据，缺失的数据、文献和个人信息标为待补。

## 文件结构

```text
tju-master-thesis/
├── SKILL.md                         # 技能入口和工作方式
├── agents/openai.yaml               # 技能显示名称与调用提示
├── references/
│   ├── format-rules.md              # 格式参数和结构要求
│   ├── writing-workflow.md          # 写作、润色、摘要与引用
│   ├── source-and-title-pages.md    # 版本、扉页、声明及歧义
│   └── review-checklist.md          # 检查项目和问题报告
└── assets/tju-format-source.docx    # 原始规定及附件
```

## 安装

将整个仓库目录保存为 `~/.codex/skills/tju-master-thesis`，确保入口路径为 `~/.codex/skills/tju-master-thesis/SKILL.md`。若设置了自定义 `CODEX_HOME`，则放入其 `skills/tju-master-thesis` 目录。

## 使用

在 Codex 中提供研究材料或论文文件，并指定任务，例如：

> 使用 $tju-master-thesis，根据我的研究材料设计硕士论文提纲，列出各章节需要补充的证据。

> 使用 $tju-master-thesis，润色这一章，保留数据、技术含义和引用编号。

> 使用 $tju-master-thesis，检查这份专业硕士论文，逐项列出问题位置、依据和修改办法。

学术硕士与专业硕士采用不同扉页；实践成果总结报告仅在明确采用该成果形式时使用对应附件。实际页码、字体、图表和分页是否符合要求，须在最终排版文件中检查。
