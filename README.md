# Latex CV by Icarus

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
