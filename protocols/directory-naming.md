**Email:** bojue.math@gmail.com\
**Version:** 1.0.0\
**Last Updated:** 2026-11-28 00

# `Directory naming protocol`

`Status` `Proposed`

## `Scope`

本仓库自有的目录名与目录组织方式。

```mermaid
flowchart LR
    resource["待归类资源"] --> parent["选择职责明确的目录"]
    parent --> child["省略已由上级表达的信息"]
    child --> check["逐级核查拼写及冲突"]
```

## `Rules`

- 普通目录使用小写 `kebab-case`，每个词段由小写 `ASCII` 字母或数字组成，词段以单个连字符分隔。目录名应表达清晰的 [`Namespace`](../dictionary/engineering-terms.md#namespace)、职责或资源集合。
- 使用简短明确的路径，省略上级路径已经表达且不会造成歧义的信息。集合目录可使用复数（如 `protocols`、`templates`）或惯用名称（如 `src`、`data`）。
- 有实际资源需要归类时再建目录。
- 路径各级名称遵循[路径可移植性规则](file-naming.md#path-portability)。

普通目录名可用 `^[a-z0-9]+(?:-[a-z0-9]+)*$` 检查字面形式。目录各级分别检查，并单独验证保留名称及同级冲突。例如，`data/raw/` 符合字面规则，`data/raw_files/` 和 `Data/raw/` 不符合。

## `Exceptions`

保留外部工具识别的目录名，如 `.github`、`.git`。需要通过 `Python` 的 `import` 语句导入的包目录使用相应的标识符形式。第三方目录保留原名。

## `Examples`

`experiments/001/results.csv` 中，`experiments/001/` 已表达实验类别和编号。若无需额外区分，可省略 `experiments/experiment-001/` 中重复的类别名称。文件名遵循[文件命名协议](file-naming.md)。

## `Verification`

核对各级名称是否符合拼写、可移植性或明确的例外，并确认同级目录职责清楚。修改现有目录名时，应依据维护授权并更新受影响的引用。
