# `Specification`

`Status` `Proposed`

## `Requirements`

在本仓库中，`MUST` 表示强制要求，`SHOULD` 表示可在有充分理由时例外的推荐做法，`MAY` 表示可选做法。

### `Dictionary entries`

- 每个概念 `MUST` 只有一个权威词条。二级 `Markdown` 标题 `MUST` 以行内代码标记规范英文术语。下一段 `MUST` 以行内代码字段 `Chinese equivalent` 开头并给出中文对应词，再下一段 `MUST` 给出简明定义。
- 词条 `SHOULD` 通过标题锚点链接相关概念，并在有助于理解时补充区别、示例或来源。重命名或迁移词条时，同步更新受影响的链接。
- 比较或依赖关系较多时，`MAY` 在定义后使用独立的 `Related terms` 段落，链接到权威词条。关系的具体含义写入定义或补充说明。
- 新增词条 `MUST` 在分类索引登记一次。归属记录以索引为准。[`Engineering taxonomy`](dictionary/taxonomy.md)

### `Protocols`

- 每份协议 `MUST` 标明状态、适用范围、规则、例外、示例和核查方式。采用模板中的英文字段、章节名和状态值，明确区分拟议与已采用的规则。[`Protocol template`](templates/protocol.md)
- 生命周期为 `Proposed → Adopted → Deprecated`。维护者确认适用范围、核查结果和例外后方可采用。弃用时说明原因，并在有替代项时提供链接。
- 显式词条关系 `MUST` 使用已定义的方向和关系名。[`Semantic relationships`](dictionary/semantic-relationships.md)

### `Repository content`

- 声称某项定义或规则属于外部标准时，`MUST` 引用可核实的来源。依据可能不明确时，标明其属于常见用法或仓库约定。
- 仓库自有文本 `MUST` 使用 `UTF-8` 编码。路径 `SHOULD` 遵循命名协议及其明确列出的例外。[`File naming`](protocols/file-naming.md) · [`Directory naming`](protocols/directory-naming.md)
- 内部 `Markdown` 链接 `MUST` 使用相对路径，大小写与目标路径一致，并能解析到所引用的文件、目录或标题。
- 修改 `MUST` 保留本次任务范围以外的用户改动，核查报告须以实际执行结果为依据。

初始版本的验收条件为入口能访问已有实质内容的术语、协议和模板，内部链接均有效，且无需专用运行环境。[`README`](README.md)
