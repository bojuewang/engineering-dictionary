**Email:** bojue.math@gmail.com\
**Version:** 1.0.0\
**Last Updated:** 2026-11-28 00

# `Engineering taxonomy`

- **并列**：从同一个类别发出的箭头表示分类归属。每个词条只归入一类。
- **平行**：虚线连接可以从不同角度对照的概念。
- **有向关系**：词条之间带标签的箭头按起点到终点阅读。跨类别关系见[术语关系图](semantic-relationships.md)。

## `Systems and design`

系统的组成、边界、表示及交互能力。

```mermaid
flowchart LR
    category["系统与设计"]
    category --> system["System"]
    category --> component["Component"]
    category --> architecture["Architecture"]
    category --> interface["Interface"]
    category --> implementation["Implementation"]
    category --> configuration["Configuration"]
    category --> state["State"]
    category --> model["Model"]
    category --> interoperability["Interoperability"]
    category --> portability["Portability"]
    category --> subsystem["Subsystem"]
    category --> design["Design"]
    category --> dependency["Dependency"]
    category --> application_programming_interface["Application programming interface"]
    category --> runtime["Runtime"]
    category --> agent["Agent"]
    subsystem -->|is-a| system
    component -->|part-of| system
    application_programming_interface -->|is-a| interface
    design -->|确定| architecture
    interoperability -. 平行：协作 / 迁移 .- portability
```

<details>
<summary>打开词条链接</summary>

- [`System`](engineering-terms.md#system)
- [`Component`](engineering-terms.md#component)
- [`Architecture`](engineering-terms.md#architecture)
- [`Interface`](engineering-terms.md#interface)
- [`Implementation`](engineering-terms.md#implementation)
- [`Configuration`](engineering-terms.md#configuration)
- [`State`](engineering-terms.md#state)
- [`Model`](engineering-terms.md#model)
- [`Interoperability`](engineering-terms.md#interoperability)
- [`Portability`](engineering-terms.md#portability)
- [`Subsystem`](engineering-terms.md#subsystem)
- [`Design`](engineering-terms.md#design)
- [`Dependency`](engineering-terms.md#dependency)
- [`Application programming interface`](engineering-terms.md#application-programming-interface)
- [`Runtime`](engineering-terms.md#runtime)
- [`Agent`](engineering-terms.md#agent)

</details>

## `Requirements and governance`

工程工作所依据的需求、约束和规则。

```mermaid
flowchart LR
    category["需求与治理"]
    category --> stakeholder["Stakeholder"]
    category --> instruction["Instruction"]
    category --> audience["Audience"]
    category --> requirement["Requirement"]
    category --> constraint["Constraint"]
    category --> specification["Specification"]
    category --> standard["Standard"]
    category --> convention["Convention"]
    category --> protocol["Protocol"]
    category --> acceptance_criterion["Acceptance criterion"]
    specification -->|汇集| requirement
    acceptance_criterion -->|给出验收条件| requirement
    standard -. 平行：标准 / 约定 .- convention
```

<details>
<summary>打开词条链接</summary>

- [`Stakeholder`](engineering-terms.md#stakeholder)
- [`Instruction`](engineering-terms.md#instruction)
- [`Audience`](engineering-terms.md#audience)
- [`Requirement`](engineering-terms.md#requirement)
- [`Constraint`](engineering-terms.md#constraint)
- [`Specification`](engineering-terms.md#specification)
- [`Standard`](engineering-terms.md#standard)
- [`Convention`](engineering-terms.md#convention)
- [`Protocol`](engineering-terms.md#protocol)
- [`Acceptance criterion`](engineering-terms.md#acceptance-criterion)

</details>

## `Information and artifacts`

资源的标识、结构、来源和演变。

```mermaid
flowchart LR
    category["信息与产物"]
    category --> artifact["Artifact"]
    category --> context["Context"]
    category --> documentation["Documentation"]
    category --> identifier["Identifier"]
    category --> namespace["Namespace"]
    category --> metadata["Metadata"]
    category --> schema["Schema"]
    category --> manifest["Manifest"]
    category --> provenance["Provenance"]
    category --> repository["Repository"]
    category --> version["Version"]
    category --> release["Release"]
    category --> version_control["Version control"]
    category --> data["Data"]
    category --> serialization["Serialization"]
    category --> source_code["Source code"]
    category --> prompt["Prompt"]
    category --> baseline["Baseline"]
    metadata -->|描述| data
    manifest -->|可包含| metadata
    provenance -->|记录来源| artifact
    release -->|is-a| version
    version_control -->|记录| version
    serialization -->|转换表示| data
    metadata -. 平行：描述 / 约束 .- schema
```

<details>
<summary>打开词条链接</summary>

- [`Artifact`](engineering-terms.md#artifact)
- [`Context`](engineering-terms.md#context)
- [`Documentation`](engineering-terms.md#documentation)
- [`Identifier`](engineering-terms.md#identifier)
- [`Namespace`](engineering-terms.md#namespace)
- [`Metadata`](engineering-terms.md#metadata)
- [`Schema`](engineering-terms.md#schema)
- [`Manifest`](engineering-terms.md#manifest)
- [`Provenance`](engineering-terms.md#provenance)
- [`Repository`](engineering-terms.md#repository)
- [`Version`](engineering-terms.md#version)
- [`Release`](engineering-terms.md#release)
- [`Version control`](engineering-terms.md#version-control)
- [`Data`](engineering-terms.md#data)
- [`Serialization`](engineering-terms.md#serialization)
- [`Source code`](engineering-terms.md#source-code)
- [`Prompt`](engineering-terms.md#prompt)
- [`Baseline`](engineering-terms.md#baseline)

</details>

## `Execution and assurance`

工作的组织方式及用于评估结果的证据。

```mermaid
flowchart LR
    category["执行与核查"]
    category --> workflow["Workflow"]
    category --> pipeline["Pipeline"]
    category --> test["Test"]
    category --> measurement["Measurement"]
    category --> evidence["Evidence"]
    category --> verification["Verification"]
    category --> validation["Validation"]
    category --> traceability["Traceability"]
    category --> risk["Risk"]
    category --> hypothesis["Hypothesis"]
    category --> experiment["Experiment"]
    category --> reproducibility["Reproducibility"]
    pipeline -->|阶段化形式| workflow
    test -->|produces| evidence
    measurement -->|produces| evidence
    experiment -->|检验| hypothesis
    reproducibility -->|评估能否复现| experiment
    verification -. 平行：规定要求 / 预期用途 .- validation
```

<details>
<summary>打开词条链接</summary>

- [`Workflow`](engineering-terms.md#workflow)
- [`Pipeline`](engineering-terms.md#pipeline)
- [`Test`](engineering-terms.md#test)
- [`Measurement`](engineering-terms.md#measurement)
- [`Evidence`](engineering-terms.md#evidence)
- [`Verification`](engineering-terms.md#verification)
- [`Validation`](engineering-terms.md#validation)
- [`Traceability`](engineering-terms.md#traceability)
- [`Risk`](engineering-terms.md#risk)
- [`Hypothesis`](engineering-terms.md#hypothesis)
- [`Experiment`](engineering-terms.md#experiment)
- [`Reproducibility`](engineering-terms.md#reproducibility)

</details>

## `Knowledge organization`

知识库中记录和复用概念的形式。

```mermaid
flowchart LR
    category["知识组织"]
    category --> canonical_term["Canonical term"]
    category --> single_source_of_truth["Single Source of Truth"]
    category --> dictionary_entry["Dictionary entry"]
    category --> template["Template"]
    category --> concept["Concept"]
    category --> taxonomy["Taxonomy"]
    category --> ontology["Ontology"]
    dictionary_entry -->|记录| canonical_term
    canonical_term -->|命名| concept
    template -->|提供格式| dictionary_entry
    taxonomy -. 平行：分类 / 概念与关系 .- ontology
```

<details>
<summary>打开词条链接</summary>

- [`Canonical term`](engineering-terms.md#canonical-term)
- [`Single Source of Truth`](engineering-terms.md#single-source-of-truth)
- [`Dictionary entry`](engineering-terms.md#dictionary-entry)
- [`Template`](engineering-terms.md#template)
- [`Concept`](engineering-terms.md#concept)
- [`Taxonomy`](engineering-terms.md#taxonomy)
- [`Ontology`](engineering-terms.md#ontology)

</details>
