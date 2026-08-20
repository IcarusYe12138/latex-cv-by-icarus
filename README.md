# Latex CV by Icarus

English | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md)

![LaTeX](https://img.shields.io/badge/LaTeX-XeLaTeX-2F2FE4?style=flat-square&logo=latex&logoColor=white)
![Workflow](https://img.shields.io/badge/Workflow-Agent--Driven-2F2FE4?style=flat-square)
![Bilingual](https://img.shields.io/badge/Bilingual-中文%20%7C%20English-2F2FE4?style=flat-square)
![Templates](https://img.shields.io/badge/Templates-Advertising%20%7C%20PR-2F2FE4?style=flat-square)
![Validation](https://img.shields.io/badge/Validation-Compile%20%2B%20Extract%20PDF-2F2FE4?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-2F2FE4?style=flat-square)

Prebuilt LaTeX resume templates and an agent-driven workflow for turning raw resume content into polished, job-ready CVs.

`Latex CV by Icarus` is a resume-building skill that combines reusable LaTeX templates with an agent-guided workflow. It helps transform raw or evolving resume content into polished, application-ready CVs through structured iteration, layout control, validation checks, and delivery conventions.

Rather than being just a static template repository, this project works as a complete CV production system. The templates define the formatting standard, while the workflow helps refine content, improve alignment with job requirements, manage page length, and ensure the final output is clean, consistent, and ready to deliver.

## Preview

These are rendered PNG previews of the current template set.

<p>
  <img src="assets/previews/A-广告-中文-1.png" alt="Advertising template in Simplified Chinese" width="48%" />
  <img src="assets/previews/A-广告-英文-1.png" alt="Advertising template in English" width="48%" />
</p>
<p>
  <img src="assets/previews/P-公关-中文-1.png" alt="PR template in Simplified Chinese" width="48%" />
  <img src="assets/previews/P-公关-英文-1.png" alt="PR template in English" width="48%" />
</p>

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

## Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/IcarusYe12138/latex-cv-by-icarus.git
cd latex-cv-by-icarus

# 2. Pick a template from assets/templates/ (A/P × ZH/EN)

# 3. Prepare your Markdown resume as the content source

# 4. Compile with XeLaTeX
latexmk -xelatex A-广告-中文.tex

# 5. Validate the output
pdftotext A-广告-中文.pdf - | head
```

For a full agent-driven experience, install this skill into your TRAE/Codex-style agent and ask it to render a Markdown resume into one of the four prepared templates. The agent will manage template selection, structural mapping, layout tuning, and validation.

## Use Cases

- **Targeted applications** — adapt the same Markdown source to different roles by iterating on highlights, ordering, and emphasis
- **Bilingual production** — maintain one content source and render Chinese (1 page) and English (2 pages) outputs side by side
- **Ad / PR focus** — pick the A or P template family and let the agent align content with the target direction
- **Page-length control** — fix “one-page” or “two-page” issues using the documented tuning ladder without deleting content
- **Recurring submissions** — re-run the same workflow for every new role with consistent output quality

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
