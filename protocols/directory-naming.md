# `Directory naming protocol`

`Status` `Proposed`

## `Scope`

本仓库自有的目录名与目录组织方式。

## `Rules`

- 普通目录使用小写 `kebab-case`，每个词段由小写 `ASCII` 字母或数字组成，词段以单个连字符分隔。目录名应表达清晰的 [`Namespace`](../dictionary/engineering-terms.md#namespace)、职责或资源集合。
- 使用简短明确的路径，省略上级路径已经表达且不会造成歧义的信息。集合目录可使用复数（如 `protocols`、`templates`）或惯用名称（如 `src`、`data`）。
- 有实际资源需要归类时再建目录。
- 路径各级名称遵循[路径可移植性规则](file-naming.md#path-portability)。

普通目录名可用 `^[a-z0-9]+(?:-[a-z0-9]+)*$` 检查字面形式。目录各级分别检查，并单独验证保留名称及同级冲突。例如，`data/raw/` 符合字面规则，`data/raw_files/` 和 `Data/raw/` 不符合。

## `Exceptions`

保留外部工具识别的目录名，如 `.github`、`.git`。需要通过 `Python` 的 `import` 语句导入的包目录使用相应的标识符形式。第三方目录保留原名。

## `Examples`

```text
research-project/
  data/
    raw/
    processed/
  experiments/
    001/
      configuration.json
      results.json
```

`experiments/001/` 已表达实验编号。如无额外区分需要，可省略 `experiments/experiment-001/` 中重复的类别名称。目录中资源的文件名遵循[文件命名协议](file-naming.md)。

## `Verification`

核对各级名称是否符合拼写、可移植性或明确的例外，并确认同级目录职责清楚。修改现有目录名时，应依据维护授权并更新受影响的引用。
