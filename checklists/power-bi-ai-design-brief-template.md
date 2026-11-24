# Power BI design brief for an AI tool

Think like a designer | Juliana Smith | Data Days | aka.ms/DataDays

How to use: edit everything in [square brackets], delete the lines you do not need, then paste the whole brief into Copilot, ChatGPT, Claude or any other AI tool. Keep your own metrics, data model and visual choices in section 1. The accessibility rules in section 7 can be replaced with the output of the Accessibility Prompt Builder (pbiaudits.com/accessibility-prompt-builder).

A prompt improves the starting point. It does not replace testing: always check the result yourself (section 9).

---

## 0. Role and task

Role: You are a Power BI report designer and accessibility reviewer.
Task: [Propose a one-page layout for ... / Build a page that ...]
Output: [A layout plan, then the alt text for each visual / A Power BI theme JSON / ...]

## 1. Requirements (what people need, not which chart to use)

Who uses it: [role, for example regional managers]
Decision they make: [for example where to focus next month]
Where and how: [desktop, tablet, meeting room screen, printed]
Access needs: [for example screen reader users, keyboard only, low vision, colour vision deficiency]
Business questions this page must answer:
1. [Question 1]
2. [Question 2]
3. [Question 3]
Measures and data: [list the measures, tables and filters that exist. The AI must not invent any]

## 2. Canvas and scale (set this first, every size follows from it)

Canvas: [1280] x [720] px
Base: 12 pt font at a 1280 x 720 canvas.
Scale factor = new canvas height / 720
Minimum font size (pt) = 12 x scale factor, rounded up to a whole number.
Apply the same scale factor to padding, gaps, and the minimum size of buttons, slicers and icons.
Example: 1920 x 1080 gives a scale factor of 1.5, so the minimum font size is 18 pt.
Show me the calculated values before you build anything.

## 3. D: Dress (colour and branding)

Brand: [my colours, fonts and logo, or paste the hex codes]
Meaning: One colour, one meaning. These are the colour roles: [for example orange = needs attention, grey = context, blue = selected]
Palette: Palette and tints only. No new colours.
Cue: Never colour alone. Add an icon, label or pattern as a second cue.
Cards: Soft card background on the page canvas. No heavy borders.

## 4. E: Elements (visuals and layout)

Layout: [Z-pattern or F-pattern]. Title top left, key message first, detail last.
Purpose: One question per visual. Say which business question each visual answers. Cut the rest.
Limit: Maximum [7 to 8] elements per page. Count KPI cards, charts, tables and slicers. Merge or cut the rest.
Group: Related items close together. Clear gaps between groups.
Align: Snap everything to a grid. Same edges, same gaps.
Space: Consistent white space on every page. Use white space before borders.

## 5. P: Patterns (contrast, typography and design systems)

System: Use [the attached design system / my design system]. No new styles.
Contrast: 4.5:1 for text. 3:1 for large text and graphics.
Font: [Sans serif font name]. Use the minimum size from section 2.
Design system covers: colour roles, text sizes, spacing and grid, page templates, wording, accessibility.

## 6. T: Trust (hierarchy, chart honesty, assistive technology and testing)

Hierarchy: Summary sentence and [3 to 4] KPI cards first, each with a comparison. Detail below.
Focus: One focal point per page. Strongest contrast on it only. Tell me what it is.
Honest: Axes start at zero for bar charts. Same scale for charts that are compared. Label units.
Compare: Show every number against [target / last year / previous period].
Titles: State the message, not the chart type.
Alt text: Describe the insight for every visual, bound to a measure so it updates. Do not describe the chart type only.
Assumptions: List every assumption you make. I will verify the numbers and the meaning.

## 7. H: Humans (users, accessibility, interaction and navigation)

Language: Plain words. No jargon or unexplained abbreviations. Empty states say what is missing and what to do next.
Motion: Anything that moves needs a pause button.
Filters: Clear labels. Show what is selected.
Tab order: Title, filters, KPIs, then visuals. Hide decorative shapes from the tab order.
Navigation: Same menu and labels on every page.

Accessibility Prompt Builder output (optional): paste it here.
[Paste the prompt generated at pbiaudits.com/accessibility-prompt-builder]

## 8. Ask first

Before you answer, ask me up to [five] questions, one at a time. Start with anything missing from section 1 or section 2.

## 9. Check before you hand over

Ask the AI to check its own work against this list, then do the same yourself.

- [ ] Canvas size and calculated font sizes were stated and applied
- [ ] Every visual answers one of the business questions in section 1
- [ ] No more than [7 to 8] elements on the page
- [ ] One clear focal point, and it is the key message
- [ ] Text contrast is at least 4.5:1, graphics and large text at least 3:1
- [ ] Colour is never the only cue
- [ ] Every number has a comparison and a unit
- [ ] Every visual has alt text that states the insight
- [ ] Tab order follows the reading order
- [ ] Nothing moves without a pause button

Test like a user:
1. Put the mouse aside
2. Navigate with the keyboard
3. Listen with a screen reader
4. Change the filters

Skills help, testing confirms: a skill can check a rule, only people can check the meaning.
