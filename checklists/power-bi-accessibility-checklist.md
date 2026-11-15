# Power BI accessibility checklist

*Data Tides · Juliana Smith*

A practical checklist for building Power BI reports that work for everyone. It follows the four WCAG principles: perceivable, operable, understandable and robust.

Tick each item as you review a report. Each item has a tip on how to check or fix it.

---

## 1. Making content perceivable

- [ ] **The font is simple, accessible and has good character differentiation**  
  Choose sans serif fonts for clarity, such as Verdana, Arial, Calibri or Segoe UI (the Power BI default). Check that characters like "I", "l" and "1" are visually distinct.
- [ ] **All meaningful elements have sufficient contrast against the background**  
  This covers text and non-text elements such as icons and charts: 4.5:1 for regular text, 3:1 for large text and 3:1 for non-text elements. Use a colour contrast checker like the [Adobe Colour Contrast Checker](https://color.adobe.com/create/color-contrast-analyzer).
- [ ] **Critical information is not communicated by colour only**  
  Add icons, text labels or patterns in charts. Preview your report with a colour blindness simulator like [Coblis](https://www.color-blindness.com/coblis-color-blindness-simulator/), keeping data confidentiality in mind.
- [ ] **All visuals and elements are organised in a meaningful sequence**  
  Use information hierarchy: start with KPIs, then visuals, then trends. Align content to natural scanning patterns (top to bottom, left to right).
- [ ] **The report layout feels clear and uncluttered**  
  Limit visuals to 5–7 per page and use generous white space to reduce clutter and cognitive load.
- [ ] **All meaningful images, icons and visuals have alt text**  
  Write alt text that explains the key message or trend in the visual. Use DAX to create dynamic alt text.
- [ ] **All decorative elements are hidden from screen readers**  
  If an element doesn't convey meaningful information, hide it in the Tab order panel.
- [ ] **Font size is legible (e.g. titles 28–32pt, body 14–16pt)**  
  Use 28–32pt for titles, 14–16pt for body text and 12–14pt for labels. Avoid anything below 10pt, even though the default is 8pt.

## 2. Making content operable

- [ ] **All page titles, visual headings and labels are present and clearly descriptive**  
  Avoid vague names like "KPIs". Be specific about what the user is looking at, e.g. "Monthly Revenue by Region".

- [ ] **Tab order follows a logical order**  
  Under Tab order, arrange elements in the same sequence users are meant to read the report.
- [ ] **The report can be navigated with the keyboard only, with no keyboard traps**  
  Test using Tab and Enter. Can you reach every filter and visual?
- [ ] **All slicers have clear, descriptive labels**  
  Avoid vague terms like "Project". Use "Select Project" instead.
- [ ] **Buttons and slicers are large enough to click easily**  
  Click targets should be at least 44 × 44px.

## 3. Making content understandable

- [ ] **No business jargon or three-letter acronyms (TLAs) are used**  
  Use plain, audience-friendly labels. Replace jargon and TLAs like "YOY" with full terms like "Year-over-Year Change".
- [ ] **Layout and interaction patterns are consistent across report pages**  
  Use a reusable template with fixed header positions, aligned slicers and consistent navigation.
- [ ] **Brief instructions guide users where needed**  
  Add short, context-aware guidance such as "Right-click a data point to drill through" to help users read charts or use interactions. Tooltips work well, but make sure the information is also available to screen reader users.
- [ ] **Table visuals have the Row Name set under accessibility**  
  Choose the column that best identifies each row's subject, such as a name, category or label.

## 4. Making content robust

- [ ] **All tables and matrices have descriptive column headers**  
  Use clear, specific labels like "Region Name" instead of just "Region", so all users understand the data structure and context at a glance.
- [ ] **Slicer selections are clearly communicated and visible**  
  Use dynamic titles, summary cards or highlighted labels to show what's been selected. This helps all users understand the current filter context.
- [ ] **All interactive elements have a clear name and state**  
  Label buttons, slicers and other controls meaningfully (e.g. "Reset Filters"), and make sure they reflect their current state (e.g. selected, disabled).
- [ ] **The report is screen reader-friendly**  
  Test the report with a screen reader. [Windows Narrator](https://support.microsoft.com/en-us/windows/complete-guide-to-narrator-e4397a0d-ef4f-b386-d8ae-c172f109bdb1) or [NVDA](https://www.nvaccess.org/download/) are great places to start.

