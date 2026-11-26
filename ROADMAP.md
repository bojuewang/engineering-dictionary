# `Roadmap`

按验收条件推进。每一阶段以前一阶段的产出为基础。

| `Phase` | 实施内容 | 验收条件 |
| --- | --- | --- |
| `1 — Foundation and Standardization` | 建立分类索引、双语核心词条、命名协议和统一条目格式。 | 全部核心词条可从分类索引找到，命名示例和内部链接通过核查。 |
| `2 — Cross-disciplinary application` | 选取至少两个工程领域的实际资料，用同一条目格式补充案例、术语区别和来源。 | 每个领域至少有一个可复用案例，跨领域概念共用权威定义，领域差异有明确范围。 |
| `3 — Machine consumption` | 根据实际工具的输入需求，评估从 `Markdown` 生成索引或加入自动核查。 | 至少一个实际使用方可从现有词条获取所需字段，生成数据可追溯到原文。 |
| `4 — Release and maintenance` | 明确许可证、版本承诺、变更记录和维护职责。 | 维护者确认发布范围、许可及版本规则，并授权首次发布。 |

第一阶段的入口见 [`Engineering taxonomy`](dictionary/taxonomy.md)、[`Specification`](SPECIFICATION.md) 和 [`Verification report`](VERIFICATION.md)。`v0.1.0` 是第一阶段的初始公开基线。第四阶段面向后续常规发布，需进一步明确长期的兼容性和维护承诺。

## 待决事项

- 何时正式采用现有的 `Proposed` 规范和协议。
- 第二阶段采用哪些领域和实际资料。
- 是否需要稳定的外部词条标识或生成索引，由第三阶段的使用需求决定。
- 发布许可证和兼容性承诺，以及是否采用 `SemVer`。
