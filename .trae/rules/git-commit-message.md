---
alwaysApply: true
scene: git_message
---

# Git 提交信息规则（事实来源：《通用项目建项规范-SPEC》§9）

- **格式**：`<type>(<scope>): <中文 subject>`；body 可选，只写动机不写流水账，每行 ≤72 字。
- **type**：feat / fix / refactor / perf / style / docs / chore / test / revert。
- **subject**：中文祈使句，≤50 字，末尾无句号；禁止 `update`、纯英文 subject、一条提交混多种 type。
- **纪律**：只 `git add` 相关文件，禁止 `git add -A`；未经用户明确要求不提交、不 push；hook 失败后新建提交而非 amend，禁止 `--no-verify`（除非用户明确要求）。
