# `Engineering terms`

本术语表提供工程实践中的双语工作定义。涉及特定标准时，在对应词条中注明来源。按用途浏览 [`Engineering taxonomy`](taxonomy.md)，新增词条时使用 [`Term template`](../templates/term.md)。

## `Architecture`

`Chinese equivalent` 架构

系统的基本组织方式，包括组成部分及其相互关系。

## `Artifact`

`Chinese equivalent` 工件、产物

工程活动产出或维护的对象，例如文档、数据集、可执行文件或证书。相关概念为 [`Provenance`](#provenance)。

## `Canonical term`

`Chinese equivalent` 规范术语

本术语表为一个概念选定的首选英文名称。

## `Configuration`

`Chinese equivalent` 配置

用于设定系统行为的一组参数或选项。

## `Convention`

`Chinese equivalent` 约定

普遍采用或在特定范围内约定的做法。

## `Dictionary entry`

`Chinese equivalent` 词条

记录一个概念的规范术语、对应词、定义及必要补充信息的条目。[`Canonical term`](#canonical-term)

## `Identifier`

`Chinese equivalent` 标识符

在特定范围内标识某个实体的名称或符号。[`Namespace`](#namespace)

## `Implementation`

`Chinese equivalent` 实现

对规格说明或设计的具体落实。[`Specification`](#specification)

## `Interface`

`Chinese equivalent` 接口

组件之间进行交互的约定边界。

## `Interoperability`

`Chinese equivalent` 互操作性

系统或组件交换信息并使用所交换信息的能力。

## `Manifest`

`Chinese equivalent` 清单

声明包含哪些资源或组件及其相关属性的记录。清单可以包含描述各资源的元数据。[`Metadata`](#metadata)

## `Metadata`

`Chinese equivalent` 元数据

描述资源、对象或数据集的数据。

## `Namespace`

`Chinese equivalent` 命名空间

用于解释和区分标识符的范围。[`Identifier`](#identifier)

## `Pipeline`

`Chinese equivalent` 流水线

由一系列处理阶段组成的流程，前一阶段的输出通常作为后一阶段的输入。[`Workflow`](#workflow)

## `Portability`

`Chinese equivalent` 可移植性

资源可以在不同环境中使用，或只需较少修改即可迁移的程度。

## `Protocol`

`Chinese equivalent` 协议

为交互、通信或执行过程约定的一组规则。[`Convention`](#convention)

## `Provenance`

`Chinese equivalent` 来源与沿革

资源的来源及其形成和变更历史的记录。

## `Release`

`Chinese equivalent` 发布版

已向使用方提供的版本。[`Version`](#version)

## `Repository`

`Chinese equivalent` 仓库

集中管理的一组资源，通常保留变更历史。[`Version control`](#version-control)

## `Schema`

`Chinese equivalent` 模式

对数据允许采用的结构及其约束的描述。数据检查可以用模式判断实例是否满足结构约束。

## `Specification`

`Chinese equivalent` 规格说明

对实现应满足的要求和约束作出的明确说明。[`Implementation`](#implementation)

## `Standard`

`Chinese equivalent` 标准

为重复使用而制定的文件，规定要求、指南或特性。其效力取决于制定机构和采用方式。

## `State`

`Chinese equivalent` 状态

描述系统或对象在特定时点所处情况的信息。

## `Template`

`Chinese equivalent` 模板

用于生成结构一致的条目或其他产物的可复用形式。

## `Validation`

`Chinese equivalent` 有效性确认

评估系统或产物是否满足预期用途或用户需求。有些领域也用该词指数据约束检查。[`Verification`](#verification)

## `Verification`

`Chinese equivalent` 验证

评估系统或产物是否满足规定要求。[`Validation`](#validation)

## `Version`

`Chinese equivalent` 版本

资源经明确标识的某一状态。[`Release`](#release)

## `Version control`

`Chinese equivalent` 版本控制

记录资源变更，使历史版本可以识别和恢复的做法。[`Version`](#version)

## `Workflow`

`Chinese equivalent` 工作流

为达成某个结果而组织的一组活动及其依赖关系。[`Pipeline`](#pipeline)

## `Acceptance criterion`

`Chinese equivalent` 验收准则

用于判定交付物是否可以接受的可核查条件。一项需求可对应多项验收准则。

`Related terms` [`Requirement`](#requirement)

## `Component`

`Chinese equivalent` 组件

系统中可以区分、承担特定职责的组成部分。

`part-of` [`System`](#system)

## `Constraint`

`Chinese equivalent` 约束

对可选方案、设计空间或运行条件施加的限制。限制可以写入需求，例如质量不得超过指定上限。

`Related terms` [`Requirement`](#requirement)

## `Evidence`

`Chinese equivalent` 证据

用于支持或反驳某项判断的信息或记录，例如测量结果或测试记录。

`Related terms` [`Measurement`](#measurement) · [`Test`](#test)

## `Measurement`

`Chinese equivalent` 测量

通过规定的方法取得量值或观测结果的过程。

`Related terms` [`Evidence`](#evidence)

## `Model`

`Chinese equivalent` 模型

为了描述、分析或预测而对对象或过程作出的有目的的表示。

`Related terms` [`System`](#system) · [`Implementation`](#implementation)

## `Requirement`

`Chinese equivalent` 需求

系统或交付物应满足的能力、特性或条件。规格说明可以汇集多项需求。

`Related terms` [`Specification`](#specification) · [`Acceptance criterion`](#acceptance-criterion)

## `Risk`

`Chinese equivalent` 风险

不确定性对目标可能产生的影响。工程工作可结合其发生可能性和后果评估风险。

## `Stakeholder`

`Chinese equivalent` 利益相关方

能够影响工程活动、受其影响或对其结果有利益关系的个人或组织。

`Related terms` [`Requirement`](#requirement)

## `System`

`Chinese equivalent` 系统

由相互作用的组成部分构成、共同承担某项功能或实现某项目的的整体。

`Related terms` [`Component`](#component) · [`Interface`](#interface)

## `Test`

`Chinese equivalent` 测试

在规定条件下操作对象并观察结果，以取得支持评估的证据。验证也可采用检查或分析。

`Related terms` [`Evidence`](#evidence) · [`Verification`](#verification)

## `Traceability`

`Chinese equivalent` 可追溯性

通过明确的关联追踪相关记录的能力，例如从需求追踪到实现和验证证据。资源自身的来源和变更历史见相关词条。

`Related terms` [`Requirement`](#requirement) · [`Implementation`](#implementation) · [`Evidence`](#evidence) · [`Provenance`](#provenance)

## `Subsystem`

`Chinese equivalent` 子系统

在较大系统中承担可界定功能、且可作为系统分析的一部分。

`is-a` [`System`](#system)

## `Design`

`Chinese equivalent` 设计

为满足需求而确定系统结构、行为和实现方案的活动，也可指其结果。

`Related terms` [`Requirement`](#requirement) · [`Architecture`](#architecture) · [`Implementation`](#implementation)

## `Concept`

`Chinese equivalent` 概念

通过共同特征识别的一类对象、过程或性质。

`Related terms` [`Canonical term`](#canonical-term)

## `Taxonomy`

`Chinese equivalent` 分类体系

按明确准则组织类别及其归属关系的结构。

`Related terms` [`Concept`](#concept)

## `Ontology`

`Chinese equivalent` 本体

对某个领域的概念、关系及其约束作出的明确表示。

`Related terms` [`Concept`](#concept) · [`Taxonomy`](#taxonomy)

## `Dependency`

`Chinese equivalent` 依赖

一方的存在、行为或正确运行有赖于另一方的关系。

`Related terms` [`Component`](#component)

## `Data`

`Chinese equivalent` 数据

以可记录、传输或处理的形式表示的事实、测量值或其他内容。

`Related terms` [`Metadata`](#metadata) · [`Schema`](#schema)

## `Serialization`

`Chinese equivalent` 序列化

将数据结构或对象转换成可存储或传输的表示。

`Related terms` [`Data`](#data) · [`Schema`](#schema)

## `Source code`

`Chinese equivalent` 源代码

用编程语言编写、供解释、编译或进一步处理的程序文本。

`Related terms` [`Implementation`](#implementation)

## `Application programming interface`

`Chinese equivalent` 应用程序编程接口

供程序调用功能或交换信息的一组接口约定，常缩写为 `API`。

`Related terms` [`Interface`](#interface) · [`Protocol`](#protocol)

## `Runtime`

`Chinese equivalent` 运行时

支持程序执行的软件环境或服务。在时间语境中也指程序执行期间。

`Related terms` [`Implementation`](#implementation) · [`Dependency`](#dependency)

## `Agent`

`Chinese equivalent` 智能体

依据目标和可用信息选择并执行动作的系统。在人工智能应用中可调用工具推进任务。

`Related terms` [`System`](#system) · [`Workflow`](#workflow)

## `Prompt`

`Chinese equivalent` 提示

提供给模型以引导其输出或行为的输入指令或示例。

`Related terms` [`Model`](#model)

## `Hypothesis`

`Chinese equivalent` 假设

能够用观察或实验结果检验的待检验解释或推断。

`Related terms` [`Evidence`](#evidence) · [`Experiment`](#experiment)

## `Experiment`

`Chinese equivalent` 实验

在明确条件下有计划地获取观察结果，以检验假设或估计某项效应。

`Related terms` [`Hypothesis`](#hypothesis) · [`Measurement`](#measurement)

## `Reproducibility`

`Chinese equivalent` 可复现性

使用所记录的输入、方法和条件重新开展工作时，获得一致结果的程度。不同领域对复现条件的要求可能不同。

`Related terms` [`Evidence`](#evidence) · [`Provenance`](#provenance)

## `Baseline`

`Chinese equivalent` 基线

用于后续比较、评估或跟踪变更的指定参考状态。

`Related terms` [`Version`](#version) · [`Release`](#release)
