---
name: latex-cv-by-icarus
description: 提供预制 LaTeX 简历模板与一套 Agent 驱动工作流：以 Markdown 为内容源，持续迭代内容、版式与页数控制，完成编译校验、命名规范与可投递 PDF 交付。适用于“制作 LaTeX 简历”“把简历打磨到岗位要求”“压页数并输出最终 PDF”等场景。
---

# Latex CV by Icarus

用预制 LaTeX 模板和 Agent 驱动工作流，把 Markdown 简历迭代为可投递的 PDF。**Markdown 是唯一内容源，LaTeX 只负责版式**：改内容只改 MD，改格式才动 tex；Agent 负责按岗位要求持续收敛内容、版式和交付质量。

## 适用判断

- 需要把中文/英文简历 MD 渲染为最终 PDF；
- 需要调整简历版式、行距、间距、页数（压到一页或控制在两页）；
- 需要按方向（广告 A / 公关 P）套用模板或统一命名。

不做：不凭空改简历正文；不删内容来凑页数；不用真实简历内容填充模板素材。

## 核心约束

- 方向前缀：`A` = 广告/品牌/营销，`P` = 公关。
- 页面目标：中文 1 页（广告版正文 10pt、公关版 9pt）；英文 2 页（正文 11pt）。页边距统一 1.27cm。
- 字体：中文思源黑体 CN（真粗体）+ 西文 Helvetica；联系方式图标用 Tabler Icons。
- 照片：中文版放一寸照（右上角，约 2.0–2.2cm）；英文版不放照片。
- 结构：教育两行（学校+日期 / 专业+地点）、工作与项目两行（名称+日期 / 职位）、要点、技能。
- 断页纪律：开启 widow/club penalty、条目标题后 `\nopagebreak`，断页必须落在条目之间，不许切断单条要点。
- 文字可提取：保留 `\XeTeXgenerateactualtext=1`，交付前用 pdftotext 验证。
- 内容规范：数字用“1200 万+ 人次”这类中文量词写法；预计毕业统一 `(Exp.)`；避免 `%` 紧贴句号；英文冒号后首字母大写。
- 主题色默认 `#2F2FE4`（Icarus 品牌色）。如要换自己的简历主题色，到 <https://colorhunt.co/> 选一组配色，只改模板里 `\definecolor{...}{HTML}{...}` 这一行的 HEX 值（去掉 `#`），四份模板同步替换。

## 工作流

1. **内容阶段**：读取/整理 Markdown。检查结构与上述内容规范，需要调整内容时改 MD 并让用户确认，不擅自改。
2. **版式阶段**：按方向+语言从 `assets/templates/` 选模板；把 MD 结构映射为模板命令（条目、要点、技能），只做结构映射不改词句；用 XeLaTeX 编译（`latexmk -xelatex`，必要时跑两遍）。
3. **校验**：页数达标、字体嵌入（pdffonts）、文字可提取、MD 与 PDF 逐行/逐要点比对。详见 [references/编译与校验.md](references/编译与校验.md)。
4. **调参**：页数不达标时按 [references/版式与调参.md](references/版式与调参.md) 的调参阶梯只调版式；调到极限仍不行，停下回报用户选项，不删内容、不擅自改字号/边距约定。
5. **交付**：按 [references/命名与目录约定.md](references/命名与目录约定.md) 输出；改动前先备份旧文件。

## 资源

- `assets/templates/`：四份脱敏模板（A/P × 中/英）+ AI 证件照 + Tabler 字体，可整体复制使用。
- `assets/previews/`：四份模板的 PDF/PNG 预览。
- `references/版式与调参.md`：参数表、调参阶梯、“一页差一行”处理。
- `references/命名与目录约定.md`：脱敏命名公式、目录职责、备份规范。
- `references/编译与校验.md`：编译与校验命令、Tabler 图标码点。
