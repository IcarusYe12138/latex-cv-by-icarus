# Latex CV by Icarus

[English](README.md) | 简体中文 | [繁體中文](README.zh-TW.md)

预制 LaTeX 简历模板与 Agent 驱动工作流，用于把原始简历内容打磨成结构清晰、版式稳定、可直接投递的 PDF 简历。

`Latex CV by Icarus` 是一套把可复用 LaTeX 模板与 Agent 工作流结合起来的简历生产 Skill。它帮助用户从原始或持续迭代中的简历内容出发，通过结构化迭代、版式控制、校验流程与交付规范，生成更成熟的岗位投递版本。

它不是单纯的模板仓库。模板负责定义视觉与排版标准，工作流负责推动内容优化、岗位匹配、页数控制、编译校验和最终交付，让简历从“能看”走向“可投递”。

## 预览

下面是当前模板集的 PNG 渲染预览。

<p>
  <img src="assets/previews/A-广告-中文-1.png" alt="广告方向中文模板预览" width="48%" />
  <img src="assets/previews/A-广告-英文-1.png" alt="广告方向英文模板预览" width="48%" />
</p>
<p>
  <img src="assets/previews/P-公关-中文-1.png" alt="公关方向中文模板预览" width="48%" />
  <img src="assets/previews/P-公关-英文-1.png" alt="公关方向英文模板预览" width="48%" />
</p>

## 它能做什么

- 提供可复用的 LaTeX 简历模板，用于中英文简历生产
- 通过 Agent 工作流持续优化内容、结构和岗位匹配度
- 控制页数、间距、层级和整体版式一致性
- 覆盖从内容整理到最终 PDF 交付的完整流程
- 增加编译与校验步骤，确保输出不仅好看，而且可用

## 为什么做它

很多简历工具只解决“写内容”或“套模板”中的一半问题。`Latex CV by Icarus` 试图把这两件事合在一起，用可复用模板保证呈现质量，用 Agent 工作流推动持续迭代，让最终结果更接近真实求职场景中的交付标准。

## 工作流

1. 从 Markdown 简历内容出发，把它作为唯一内容源
2. 选择合适的中英模板与目标版式
3. 将内容映射到 LaTeX 结构，而不是随意改写事实
4. 借助 Agent 持续迭代，直到简历满足岗位与页数要求
5. 编译、校验并交付最终 PDF

## 仓库结构

- `SKILL.md`：Skill 定义、约束条件、工作流与操作规则
- `assets/templates/`：可复用的 LaTeX 模板、字体与示例资源
- `assets/previews/`：模板对应的 PDF 与 PNG 预览
- `references/`：命名规范、调参规则与校验说明
- `agents/openai.yaml`：Agent 集成所需的展示元信息

## 说明

- Markdown 是唯一内容源，LaTeX 负责版式与渲染
- 仓库内模板均为脱敏后的可复用生产资源
- 整体工作流强调版式纪律、校验流程与最终交付质量
