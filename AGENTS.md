# AGENTS.md · personalSpec

> 本文件是 AI 协作的**唯一统一入口**，只引导、不复制规则全文（单一事实来源原则）。

## 1. 项目定位

**通用建项规范资产库**：维护可复用的项目建项 SPEC 模板，并通过全局 skill 提供问询式立项能力。

- **主模板**：[通用项目建项规范-SPEC.md](file:///d:/g/个人项目/personalSpec/通用项目建项规范-SPEC.md) —— 四类项目形态（A 代码工程 / B 内容生成 / C 工作流搭建 / D 原型设计）的通用骨架。
- **形态接入件**：[原型设计规范-SPEC.md](file:///d:/g/个人项目/personalSpec/原型设计规范-SPEC.md) —— 形态 D 的差异部分，**只写差异**，通用骨架以主模板为准。
- **全局 skill**：`project-spec-init`（`c:\Users\ht\.trae-cn\skills\project-spec-init`）—— 封装主模板 §14 问询式立项流程，对新项目使用。

## 2. 文档索引（本项目自身按主模板最小集建项）

| 层级 | 文档 | 职责 |
| --- | --- | --- |
| L0 | AGENTS.md（本文件） | 统一入口，只引导 |
| L0 | [README.md](file:///d:/g/个人项目/personalSpec/README.md) | 人类入口：简介 + 使用方式 |
| 产品 | [通用项目建项规范-SPEC.md](file:///d:/g/个人项目/personalSpec/通用项目建项规范-SPEC.md) | 主模板（唯一通用规范源） |
| 产品 | [原型设计规范-SPEC.md](file:///d:/g/个人项目/personalSpec/原型设计规范-SPEC.md) | 形态 D 接入件 |
| L1 | [docs/README.md](file:///d:/g/个人项目/personalSpec/docs/README.md) | 本项目硬约束 + 必读流程 + 维护契约 |
| L3 | [docs/project-overview.md](file:///d:/g/个人项目/personalSpec/docs/project-overview.md) | 文件级目录地图 |
| 约定 | [docs/writing-conventions.md](file:///d:/g/个人项目/personalSpec/docs/writing-conventions.md) | SPEC 文档书写约定 |

## 3. 冲突裁决

- 主模板 ↔ 形态接入件：**以主模板为准**；接入件只允许定义该形态的差异部分。
- 本项目治理冲突：以 [docs/README.md](file:///d:/g/个人项目/personalSpec/docs/README.md) 硬约束清单为准。
- 发现文档之间或文档与实际不一致：**先报告用户裁决，不得静默采信任何一方**。

## 4. 接需求必读流程（未完成不得改文件）

1. Read 本文件 + [docs/README.md](file:///d:/g/个人项目/personalSpec/docs/README.md) 硬约束清单。
2. 修改 SPEC 产品文档：通读对应 SPEC 全文 + [docs/writing-conventions.md](file:///d:/g/个人项目/personalSpec/docs/writing-conventions.md)。
3. 定位文件先查 [docs/project-overview.md](file:///d:/g/个人项目/personalSpec/docs/project-overview.md)，**禁止全量扫描**。
4. 例外：单行 typo / 单行修复可简化，但仍须遵守硬约束。

## 5. 硬性边界（NEVER）

- **NEVER** 未经问询确认直接为新项目生成文档——立项必须走 `project-spec-init` 的问询流程。
- **NEVER** 在本文件、skill 或其他文档中复制 SPEC 规则全文——只指向唯一事实来源。
- **NEVER** 删除 SPEC 中的修订记录、否决专区、superseded 的 ADR（演进轨迹只增不删）。
- **NEVER** 主动新建 `*.md`，除非用户明确要求。
- **NEVER** `git add -A`、提交 `.env` / 临时脚本；未经用户明确要求不提交、不 push。

## 6. Git 提交

格式 `<type>(<scope>): <中文 subject>`，细则见 [.trae/rules/git-commit-message.md](file:///d:/g/个人项目/personalSpec/.trae/rules/git-commit-message.md) 与主模板 §9。

## 7. 模板演进（回填义务）

在任何项目中使用本模板发现新的硬约束、流程改进或新的项目形态时，**回填对应 SPEC**（主模板或接入件），并在修订记录中留痕；涉及章节结构变化时同步更新 `project-spec-init` skill。
