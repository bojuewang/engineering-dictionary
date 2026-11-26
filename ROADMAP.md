# `Roadmap`

```mermaid
flowchart LR
    foundation["基础 v0.1.0"] --> application["真实任务试用"]
    application -->|有实际使用方时| tools["索引或自动检查"]
    application -->|根据使用反馈| maintenance["规则采用与发布维护"]
```

1. **基础**　`v0.1.0` 已发布。术语、索引和命名约定可用。[基线核查](VERIFICATION.md)
2. **应用**　在至少两个真实工程任务中试用。把反复遇到的问题整理成可复用示例。
3. **工具**　有实际使用方时，再从现有 `Markdown` 生成索引或增加自动检查。
4. **维护**　确定后续发布的许可证、兼容性承诺和维护职责。按使用反馈决定哪些拟议规则正式采用。
