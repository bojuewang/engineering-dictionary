# `Specification`

`Status` `Proposed`

## `Requirements`

```mermaid
flowchart LR
    content["仓库内容"] -->|词条| entries["词条格式与索引"]
    content -->|协议| protocols["状态、规则与核查"]
    content -->|图表| diagrams["有向图约定"]
```

### `Dictionary entries`

每个概念只有一个权威词条。依次写英文二级标题、`Chinese equivalent` 和中文定义，并在分类索引登记一次。用 `Related terms` 链接有用的关联。显式关系使用约定的名称和方向。[词条模板](templates/term.md) · [分类索引](dictionary/taxonomy.md) · [关系](dictionary/semantic-relationships.md)

### `Protocols`

按模板记录状态、范围、规则、例外、示例和核查方式。维护者审核后可由 `Proposed` 改为 `Adopted`。标为 `Deprecated` 时说明原因，附上已有的替代方案。[协议模板](templates/protocol.md)

### `Repository content`

引用外部标准时注明来源。文本用 `UTF-8`，内部链接用大小写准确的相对路径。命名遵循协议及其例外。提交前实际核对链接、编码和命名。[文件命名](protocols/file-naming.md) · [目录命名](protocols/directory-naming.md)

### `Directed diagrams`

- 使用 `Mermaid flowchart`。默认从左向右阅读。节点使用现有术语、文件名或步骤名。
- 实线箭头从来源指向目标。按图的用途标明归属、导航、步骤或语义关系。同一来源下的分支表示并列。平行对照使用无箭头虚线。
- 分类、定义和规则以正文为准。图旁保留普通链接供查阅全文。图表改动需核对节点、箭头方向和对应链接。

### `Document layout`

文档左上角依次放置以下三行。分页输出在每页左上角重复显示，时间戳和版本在同一修订的所有页面保持一致。

```text
页码 1/12
时间戳 2026-11-27T14:35:08-05:00
版本 v1.0.0
```

- 页码采用 `x/xx`，其中 `x` 为从 `1` 开始的当前页，`xx` 为排版完成后的总页数。未分页的 Markdown 在文首写 `页码 1/1`。导出时按实际分页更新页码。
- 时间戳记录文档最近一次内容更新的时间，采用 `YYYY-MM-DDTHH:mm:ss±HH:mm`，精确到秒，并保留 UTC 偏移。
- 文档版本从 `v1.0.0` 开始。后续更新按时间戳所示当地日期与上次修订日期的关系递增。[文档修订版本](protocols/versioning.md#document-revision-version)
