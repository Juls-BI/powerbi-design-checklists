# Power BI design checklists

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](LICENSE)
[![WCAG 2.2](https://img.shields.io/badge/WCAG-2.2-220e4b.svg)](https://www.w3.org/WAI/standards-guidelines/wcag/)
[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?logo=powerbi&logoColor=black)](https://learn.microsoft.com/en-us/power-bi/create-reports/desktop-accessibility-overview)
[![Format: Markdown](https://img.shields.io/badge/Format-Markdown-000000?logo=markdown&logoColor=white)](checklists/)
[![Last commit](https://img.shields.io/github/last-commit/Juls-BI/powerbi-design-checklists)](https://github.com/Juls-BI/powerbi-design-checklists/commits/main)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](https://github.com/Juls-BI/powerbi-design-checklists/issues)

Practical, tickable checklists for designing clear, honest and accessible Power BI reports, by [Juliana Smith](https://www.linkedin.com/in/juliana-smith-citp/) at [Data Tides](https://data-tides.com/).

Each checklist is a plain Markdown file, so it works with screen readers, renders as tickable checkboxes on GitHub, and is easy to copy into your own tools.

## Start here: the DEPTH checklist

AI can build a Power BI report in minutes, but if you publish it, you own the design. The **DEPTH checklist** reviews a report across five layers, like an iceberg. Dress and Elements sit above the water, where people notice them first. Below it are the decisions that make a report work for real people.

| Layer | Covers | Question to ask |
|---|---|---|
| **D: Dress** | Colour and branding | Does it look on-brand and consistent? |
| **E: Elements** | Visuals and layout | Does every visual earn its place? |
| **P: Patterns** | Contrast, typography and design systems | Can everyone read and tell it apart? |
| **T: Trust** | Hierarchy, chart honesty, assistive technology and testing | Does it give an honest, clear message? |
| **H: Humans** | Users, accessibility, interaction and navigation | Does it work for the people who use it? |

[Open the Power BI DEPTH checklist](checklists/power-bi-depth-checklist.md). It also includes checks for dashboards built with Claude, and a sign-off section so a person, not a tool, confirms the report is ready to publish.

## Checklists

| Checklist | What it's for |
|---|---|
| [Power BI DEPTH checklist](checklists/power-bi-depth-checklist.md) | A full design review across five layers: Dress, Elements, Patterns, Trust and Humans |
| [Power BI chart selection checklist](checklists/power-bi-chart-selection-checklist.md) | Choosing a visual that answers the question and suits the data |
| [Power BI chart honesty checklist](checklists/power-bi-chart-honesty-checklist.md) | Making sure a visual gives an honest impression of the data: scales, time periods, aggregation and wording |
| [Power BI accessibility checklist](checklists/power-bi-accessibility-checklist.md) | Reviewing a whole report against the four WCAG principles: perceivable, operable, understandable and robust |
| [Power BI alt text creation checklist](checklists/power-bi-alt-text-checklist.md) | Writing static and dynamic alt text that explains the insight in each visual |

## How to use them

- **Review a report:** open a checklist on GitHub and work through it, or copy it into an issue or pull request so you can tick items as you go.
- **Add it to your team's process:** copy the Markdown into your wiki, Azure DevOps, Notion or Obsidian. Checkboxes work in all of them.
- **Give it to an AI tool:** paste a checklist into your prompt or save it as reusable instructions, then review what the AI produces against it. AI can help you check, but a person still signs off.

## Related tools

- [PBIX A11y](https://pbiaudits.com/): a free, browser-based accessibility checker for .pbix files
- [pbir-a11y](https://github.com/Juls-BI/pbir-a11y): accessibility checks for PBIP projects, pipelines and AI agents
- [Power BI Alt Text UDF Library](https://github.com/Juls-BI/powerbi-alttext-udfs): DAX user-defined functions for dynamic alt text
- [Power BI Luminance & Colour Contrast Checker](https://github.com/Juls-BI/powerbi-luminance-contrast-checker): WCAG contrast ratios in pure DAX

## Feedback

Suggestions and corrections are welcome. Please [open an issue](https://github.com/Juls-BI/powerbi-design-checklists/issues).

## License

These checklists are licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). You can share and adapt them, including for commercial use, as long as you credit **Juliana Smith, Data Tides** and link back to this repository.
