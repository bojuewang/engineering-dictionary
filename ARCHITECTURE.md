# `Architecture`

## 组织原则

术语、规则、模板和实现分别存放。每个概念只有一个权威词条，其他文档通过链接引用。[`Dictionary entry`](dictionary/engineering-terms.md#dictionary-entry)

```text
engineering-dictionary/
├── .gitattributes
├── .gitignore
├── AGENTS.md
├── ARCHITECTURE.md
├── CHANGELOG.md
├── README.md
├── ROADMAP.md
├── SPECIFICATION.md
├── VERIFICATION.md
├── dictionary/
│   ├── engineering-terms.md
│   ├── semantic-relationships.md
│   └── taxonomy.md
├── protocols/
│   ├── directory-naming.md
│   ├── file-naming.md
│   ├── naming-conventions.md
│   └── versioning.md
└── templates/
    ├── protocol.md
    └── term.md
```

| `Layer` | 职责 | `Location` |
| --- | --- | --- |
| `Terminology` | 定义概念和术语。 | [`dictionary/`](dictionary/) |
| `Taxonomy` | 记录词条的主要归属。 | [`Taxonomy`](dictionary/taxonomy.md) |
| `Semantic relationships` | 记录关系含义、方向与词条引用。 | [`Semantic relationships`](dictionary/semantic-relationships.md) |
| `Protocols` | 记录适用的规则与例外。 | [`protocols/`](protocols/) |
| `Templates` | 提供编写词条和协议的格式。 | [`templates/`](templates/) |
| `Applications` | 存放实际用例和具体实现。 | 有实际资源时单独建目录。 |
| `Automation` | 将已验证的规则用于重复执行。 | 有明确使用需求时再加入。 |

协议引用所用术语，模板引用相应的内容要求，实现引用所依据的规则。各层通过链接复用内容，定义、规则或格式只在其归属处维护。

分类索引只维护词条的主要归属和导航链接。词条本身维护定义和概念关系。[`Engineering taxonomy`](dictionary/taxonomy.md)

术语表目前集中维护。需要按主题拆分时，保留规范术语并同步更新指向迁移词条的链接。供读者和解析器使用的 `Markdown` 结构见 [`Specification`](SPECIFICATION.md)。有明确使用方时再增加独立模式或工具。历史记录按 [`Versioning`](protocols/versioning.md) 维护。
