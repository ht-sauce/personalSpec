# personalSpec · 通用建项规范资产库

维护一套可复用的项目建项 SPEC 模板，并通过全局 skill 提供**问询式立项**能力。AI 协作入口与完整规则见 [AGENTS.md](AGENTS.md)。

## 资产清单

| 文档 | 说明 |
| --- | --- |
| [通用项目建项规范-SPEC.md](通用项目建项规范-SPEC.md) | 主模板 v2.0：文档体系、硬约束机制、工作流、维护契约、ADR、§14 问询式立项；覆盖 A 代码工程 / B 内容生成 / C 工作流搭建 / D 原型设计四类形态 |
| [原型设计规范-SPEC.md](原型设计规范-SPEC.md) | 形态 D 接入件 v1.0：三层产物模型、原型类硬约束（HC-D1…16）、形态 D 专属问项 |

## 如何使用

在新项目中对 AI 说：

> 按通用建项规范帮我立项

全局 skill `project-spec-init` 会被触发：AI 通读 SPEC → 分轮带选项问询 → 输出立项纪要待确认 → 一次性生成该项目的最小规范文档集（AGENTS.md / docs/README / project-overview / 约定文档）。

## 维护

- 规范使用中发现新约束或流程改进 → 回填对应 SPEC 并在修订记录留痕（详见 [AGENTS.md](AGENTS.md) §7）。
- 本项目自身的治理文档在 [docs/](docs/)。
