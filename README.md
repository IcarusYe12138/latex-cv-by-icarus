# Latex CV by Icarus

English | [简体中文](#简体中文) | [繁體中文](#繁體中文)

Prebuilt LaTeX resume templates and an agent-driven workflow for turning raw resume content into polished, job-ready CVs.

`Latex CV by Icarus` is a resume-building skill that combines reusable LaTeX templates with an agent-guided workflow. It helps transform raw or evolving resume content into polished, application-ready CVs through structured iteration, layout control, validation checks, and delivery conventions.

Rather than being just a static template repository, this project works as a complete CV production system. The templates define the formatting standard, while the workflow helps refine content, improve alignment with job requirements, manage page length, and ensure the final output is clean, consistent, and ready to deliver.

## What It Does

- Provides prebuilt LaTeX CV templates for structured resume production
- Uses an agent workflow to iteratively improve resume quality against role requirements
- Helps manage page length, spacing, hierarchy, and formatting consistency
- Supports a production-style workflow from content shaping to final PDF delivery
- Adds validation steps so the final resume is not only visually polished but also operationally usable

## Why It Exists

Most resume tools stop at either writing assistance or visual templates. `Latex CV by Icarus` bridges both: it combines strong visual templates with an agent-guided workflow that helps continuously shape a CV until it matches real application needs.

The goal is not just to generate a nice-looking document, but to build a repeatable workflow for producing high-quality, role-aligned, delivery-ready resumes.

## Workflow

1. Start from Markdown resume content as the source of truth
2. Select the right bilingual template and target layout
3. Map content into LaTeX structures without rewriting facts arbitrarily
4. Iterate with the agent until the CV fits role requirements and page constraints
5. Compile, validate, and deliver a clean PDF output

## Repository Structure

- `SKILL.md`: skill definition, constraints, workflow, and operating rules
- `assets/templates/`: reusable LaTeX templates, fonts, and sample assets
- `assets/previews/`: PDF and PNG previews of the prepared template set
- `references/`: naming conventions, tuning rules, and validation instructions
- `agents/openai.yaml`: display metadata for agent integrations

## Notes

- Markdown is treated as the primary content source, while LaTeX handles layout and rendering
- The included templates are anonymized and intended as reusable production assets
- The workflow prioritizes formatting discipline and validation over ad hoc document editing

## 简体中文

`Latex CV by Icarus` 是一套以英文叙述为主、同时支持中文语境理解的简历生产 Skill。它把可复用的 LaTeX 模板与 Agent 驱动工作流结合起来，帮助用户将原始或持续迭代中的简历内容打磨成结构清晰、版式稳定、可以直接投递的 PDF 简历。

这个项目不是单纯的模板仓库。模板负责定义视觉与排版标准，工作流负责推动内容优化、岗位匹配、页数控制、编译校验和最终交付，让简历从“能看”走向“可投递”。

### 它能做什么

- 提供可复用的 LaTeX 简历模板，用于中英文简历生产
- 通过 Agent 工作流持续优化内容、结构和岗位匹配度
- 控制页数、间距、层级和整体版式一致性
- 覆盖从内容整理到最终 PDF 交付的完整流程
- 增加编译与校验步骤，确保输出不仅好看，而且可用

### 为什么做它

很多简历工具只解决“写内容”或“套模板”中的一半问题。`Latex CV by Icarus` 试图把这两件事合在一起，用可复用模板保证呈现质量，用 Agent 工作流推动持续迭代，让最终结果更接近真实求职场景中的交付标准。

### 工作流

1. 从 Markdown 简历内容出发，把它作为唯一内容源
2. 选择合适的中英模板与目标版式
3. 将内容映射到 LaTeX 结构，而不是随意改写事实
4. 借助 Agent 持续迭代，直到简历满足岗位与页数要求
5. 编译、校验并交付最终 PDF

### 仓库结构

- `SKILL.md`：Skill 定义、约束条件、工作流与操作规则
- `assets/templates/`：可复用的 LaTeX 模板、字体与示例资源
- `assets/previews/`：模板对应的 PDF 与 PNG 预览
- `references/`：命名规范、调参规则与校验说明
- `agents/openai.yaml`：Agent 集成所需的展示元信息

## 繁體中文

`Latex CV by Icarus` 是一套以英文敘述為主、同時支援中文語境理解的履歷生產 Skill。它把可重複使用的 LaTeX 模板與 Agent 驅動工作流結合起來，幫助使用者將原始或持續迭代中的履歷內容打磨成結構清晰、版式穩定、可直接投遞的 PDF 履歷。

這個專案不是單純的模板倉庫。模板負責定義視覺與排版標準，工作流負責推動內容優化、職缺匹配、頁數控制、編譯校驗與最終交付，讓履歷從「能看」走向「可投遞」。

### 它能做什麼

- 提供可重複使用的 LaTeX 履歷模板，用於中英文履歷生產
- 透過 Agent 工作流持續優化內容、結構與職缺匹配度
- 控制頁數、間距、層級與整體版式一致性
- 覆蓋從內容整理到最終 PDF 交付的完整流程
- 增加編譯與校驗步驟，確保輸出不只好看，也真正可用

### 為什麼做它

很多履歷工具只解決「寫內容」或「套模板」其中一半的問題。`Latex CV by Icarus` 想把這兩件事結合起來，用可重複使用的模板保證呈現品質，用 Agent 工作流推動持續迭代，讓最終結果更接近真實求職情境中的交付標準。

### 工作流

1. 從 Markdown 履歷內容出發，將其作為唯一內容來源
2. 選擇合適的中英模板與目標版式
3. 將內容映射到 LaTeX 結構，而不是任意改寫事實
4. 借助 Agent 持續迭代，直到履歷滿足職缺與頁數要求
5. 編譯、校驗並交付最終 PDF

### 倉庫結構

- `SKILL.md`：Skill 定義、約束條件、工作流與操作規則
- `assets/templates/`：可重複使用的 LaTeX 模板、字體與示例資源
- `assets/previews/`：模板對應的 PDF 與 PNG 預覽
- `references/`：命名規範、調參規則與校驗說明
- `agents/openai.yaml`：Agent 整合所需的展示中繼資料
