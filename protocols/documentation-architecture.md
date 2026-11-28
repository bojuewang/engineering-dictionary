**Email:** bojue.math@gmail.com\
**Version:** 1.0.0\
**Last Updated:** 2026-11-28 00

# `Documentation architecture protocol`

`Status` `Proposed`

## `Scope`

为人类和智能体共同参与的工程与研究仓库组织项目说明、上下文、操作指令和共享资料。适用条件与职责见[规范](../SPECIFICATION.md#audience-oriented-documentation-architecture)。

## `Rules`

1. 从人类首页的实际使用场景出发，保留项目介绍、常用入口与共享资料链接。
2. 从 [AGENTS.md](../AGENTS.md) 显式链接 [README__agents.md](../README__agents.md)。通过实际链接建立可发现性。操作义务写入适用的指令文件。
3. 按[唯一事实来源](../dictionary/engineering-terms.md#single-source-of-truth)维护共享资料。改动要求时更新规范，改动结果时更新对应核查记录，并检查引用这些内容的摘要。
4. 使用准确的相对路径。首页图及旁边的链接应能从两个受众入口定位共享资料。

## `Exceptions`

规模小且背景简明的仓库可用普通 README 提供上下文。子系统可以保有自己的权威文档与作用域指令，入口通过链接提供定位。

## `Examples`

本仓库的 [README.md](../README.md) 提供速查入口，[README__agents.md](../README__agents.md) 说明如何定位词条、协议和核查记录。例如，命名约定的正式依据仍是[文件命名协议](file-naming.md)，两条阅读路径都可到达该协议。

## `Verification`

从两个入口分别沿链接查找同一份规范和核查记录。检查指令入口是否直接链接上下文，文件名和链接大小写是否准确，图中的箭头是否符合阅读路径。比对摘要与权威来源，核对验证结论是否有对应证据，并将范围、方法与限制写入[核查记录](../VERIFICATION.md)。
