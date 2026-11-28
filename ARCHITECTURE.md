**Email:** bojue.math@gmail.com\
**Version:** 1.0.0\
**Last Updated:** 2026-11-28 00

# `Architecture`

```mermaid
flowchart LR
    taxonomy["分类索引"] -->|索引| glossary["权威词条"]
    relationships["概念关系"] -->|引用| glossary
    protocols["工作协议"] -->|引用| glossary
    templates["模板"] -->|遵循| spec["文档规范"]
```

- [`dictionary/`](dictionary/) 保存权威定义、分类索引和关系。一个概念只定义一次，其他文档链接到词条。
- [`protocols/`](protocols/) 保存工作规则。[`templates/`](templates/) 保存对应的可复制格式。
- 根目录负责导航、维护与发布。实际用例或工具有明确需求时再独立存放。

移动词条时更新引用。词条与协议格式见 [`Specification`](SPECIFICATION.md)。

## `Audience-oriented documentation architecture`

[README.md](README.md) is the human entry point. [AGENTS.md](AGENTS.md) is the operational entry point for agents and links directly to [README__agents.md](README__agents.md) for context. Both reading paths lead to shared sources, as shown in the [navigation diagram](README.md).

Each fact, rule, plan, or verification claim has one authoritative home. Audience-specific documents summarize what readers need to get started and link to the owner for details. Update the owner first when information changes, then check the affected links and summaries. See the [responsibility and ownership rules](SPECIFICATION.md#audience-oriented-documentation-architecture).
