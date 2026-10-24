# project-overview · personalSpec 文件地图

> 定位文件先查本地图，锁定后只精读目标文件，禁止全量扫描。每个文件一行职责。

## 目录树

```
personalSpec/
├─ AGENTS.md                       # AI 协作统一入口：项目定位 / 文档索引 / 冲突裁决 / NEVER 边界
├─ README.md                       # 人类入口：资产清单与使用方式
├─ 通用项目建项规范-SPEC.md          # 【产品】主模板 v3.2，四类形态通用建项骨架（唯一通用规范源）
├─ 代码工程规范-SPEC.md             # 【产品】形态 A 接入件 v1.0，代码工程专属细则 + 形态 A 问项
├─ 原型设计规范-SPEC.md             # 【产品】形态 D 接入件 v2.0，原型设计项目差异部分
├─ SPEC 修订分析附录.md             # 【产品】修订分析留档：对比分析 + 历史修订分析（只增不删）
├─ docs/
│  ├─ README.md                    # 本项目治理入口：必读流程 / 硬约束 11 条 / 维护契约
│  ├─ project-overview.md          # 本文件：文件级目录地图
│  └─ writing-conventions.md       # 产品 SPEC 的书写约定（版本 / 占位符 / 硬约束写法 / 图表表格）
└─ .trae/
   └─ rules/
      └─ git-commit-message.md     # 平台适配层：Git 提交信息规则（alwaysApply 注入）
```

## 改动类型速查

| 想做什么 | 先看哪里 |
| --- | --- |
| 给新项目立项 | 把主模板（+ 对应接入件）交给 AI，走主模板 §9 问询式立项（不在本项目内生成） |
| 改通用建项规则 | 通用项目建项规范-SPEC.md 全文 + writing-conventions.md |
| 改代码工程细则 | 代码工程规范-SPEC.md + 主模板适用范围章节 |
| 改原型设计差异规则 | 原型设计规范-SPEC.md + 主模板适用范围章节 |
| 查历史修订依据 | SPEC 修订分析附录.md（只增不删） |
| 新增形态接入件 | docs/README.md 维护契约 + AGENTS.md 索引区 |
