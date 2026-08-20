# Latex CV by Icarus

[English](README.md) | [简体中文](README.zh-CN.md) | 繁體中文

![LaTeX](https://img.shields.io/badge/LaTeX-XeLaTeX-2F2FE4?style=flat-square&logo=latex&logoColor=white)
![Workflow](https://img.shields.io/badge/Workflow-Agent--Driven-2F2FE4?style=flat-square)
![Bilingual](https://img.shields.io/badge/Bilingual-中文%20%7C%20English-2F2FE4?style=flat-square)
![Templates](https://img.shields.io/badge/Templates-廣告%20%7C%20公關-2F2FE4?style=flat-square)
![Validation](https://img.shields.io/badge/Validation-編譯%20%2B%20文字提取-2F2FE4?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-2F2FE4?style=flat-square)

預製 LaTeX 履歷模板與 Agent 驅動工作流，用於把原始履歷內容打磨成結構清晰、版式穩定、可直接投遞的 PDF 履歷。

`Latex CV by Icarus` 是一套把可重複使用的 LaTeX 模板與 Agent 工作流結合起來的履歷生產 Skill。它幫助使用者從原始或持續迭代中的履歷內容出發，透過結構化迭代、版式控制、校驗流程與交付規範，產出更成熟的職缺投遞版本。

它不是單純的模板倉庫。模板負責定義視覺與排版標準，工作流負責推動內容優化、職缺匹配、頁數控制、編譯校驗與最終交付，讓履歷從「能看」走向「可投遞」。

## 預覽

下面是目前模板集的 PNG 渲染預覽。

<p>
  <img src="assets/previews/A-广告-中文-1.png" alt="廣告方向中文模板預覽" width="48%" />
  <img src="assets/previews/A-广告-英文-1.png" alt="廣告方向英文模板預覽" width="48%" />
</p>
<p>
  <img src="assets/previews/P-公关-中文-1.png" alt="公關方向中文模板預覽" width="48%" />
  <img src="assets/previews/P-公关-英文-1.png" alt="公關方向英文模板預覽" width="48%" />
</p>

## 它能做什麼

- 提供可重複使用的 LaTeX 履歷模板，用於中英文履歷生產
- 透過 Agent 工作流持續優化內容、結構與職缺匹配度
- 控制頁數、間距、層級與整體版式一致性
- 覆蓋從內容整理到最終 PDF 交付的完整流程
- 增加編譯與校驗步驟，確保輸出不只好看，也真正可用

## 為什麼做它

很多履歷工具只解決「寫內容」或「套模板」其中一半的問題。`Latex CV by Icarus` 想把這兩件事結合起來，用可重複使用的模板保證呈現品質，用 Agent 工作流推動持續迭代，讓最終結果更接近真實求職情境中的交付標準。

## 工作流

1. 從 Markdown 履歷內容出發，將其作為唯一內容來源
2. 選擇合適的中英模板與目標版式
3. 將內容映射到 LaTeX 結構，而不是任意改寫事實
4. 借助 Agent 持續迭代，直到履歷滿足職缺與頁數要求
5. 編譯、校驗並交付最終 PDF

## 快速開始

```bash
# 1. 克隆倉庫
git clone https://github.com/IcarusYe12138/latex-cv-by-icarus.git
cd latex-cv-by-icarus

# 2. 從 assets/templates/ 中選擇模板（廣告 A / 公關 P × 中文 / 英文）

# 3. 準備好你的 Markdown 履歷作為內容來源

# 4. 使用 XeLaTeX 編譯
latexmk -xelatex A-广告-中文.tex

# 5. 校驗輸出
pdftotext A-广告-中文.pdf - | head
```

如果要走完整的 Agent 工作流，可以把本 Skill 安裝到 TRAE / Codex 這類 Agent 中，讓它把 Markdown 履歷渲染成四份預製模板之一。Agent 會負責模板選擇、結構映射、版式調參與校驗。

## 適用情境

- **針對性投遞**：圍繞同一份 Markdown 內容，針對不同職缺迭代亮點、順序與重點
- **中英雙語生產**：維護一份內容來源，同時輸出中文（1 頁）與英文（2 頁）版本
- **廣告 / 公關方向**：選擇 A 或 P 模板系列，讓 Agent 推動內容對齊目標方向
- **頁數控制**：在不刪內容的前提下，按調參階梯把履歷壓回一頁或控制在兩頁
- **重複投遞**：每次新職缺都跑同一套工作流，保證輸出品質穩定一致

## 倉庫結構

- `SKILL.md`：Skill 定義、約束條件、工作流與操作規則
- `assets/templates/`：可重複使用的 LaTeX 模板、字體與示例資源
- `assets/previews/`：模板對應的 PDF 與 PNG 預覽
- `references/`：命名規範、調參規則與校驗說明
- `agents/openai.yaml`：Agent 整合所需的展示中繼資料

## 說明

- Markdown 是唯一內容來源，LaTeX 負責版式與渲染
- 倉庫內模板均為脫敏後的可重複使用生產資源
- 整體工作流強調版式紀律、校驗流程與最終交付品質
