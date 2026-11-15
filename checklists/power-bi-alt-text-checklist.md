# Power BI alt text creation checklist

*Data Tides · Juliana Smith*

A step-by-step checklist for writing alt text that explains the insight in a Power BI visual, not just what it looks like. It starts before you open Power BI and finishes with regular reviews.

---

## 1. Understand the context (before opening Power BI)

- [ ] Identify the target audience
- [ ] Confirm whether any users rely on screen readers or other non-visual access
- [ ] Define the purpose of each visual (decision, comparison or insight)
- [ ] Check whether the report falls under the European Accessibility Act (EAA) or other EU accessibility requirements
- [ ] Consider user empathy: what must be understood without seeing the visual?

## 2. Define the insight (not the picture)

- [ ] Determine the main message of the visual
- [ ] Identify what users should understand within 3–5 seconds
- [ ] Highlight key relationships or trends
- [ ] Exclude unnecessary details
- [ ] Reassess the visual design if the insight can't be clearly summarised

## 3. Write the core alt text (static draft)

- [ ] Focus on insight, not aesthetics
- [ ] Avoid listing every data point or category
- [ ] Use plain, direct language
- [ ] State the trend, comparison or key takeaway
- [ ] Mention anomalies or important context
- [ ] Avoid jargon unless it's essential for the audience

## 4. Convert to dynamic alt text (using DAX)

- [ ] Create a DAX measure that summarises the insight dynamically
- [ ] Bind the measure to the visual's alt text using conditional formatting
- [ ] Make sure the measure updates with filters and handles blanks
- [ ] Keep sentences concise and meaningful
- [ ] Include fallback text, e.g. "No data available for the current selection."

**DAX prompts to consider:**

- [ ] Selected category
- [ ] Highest and lowest values
- [ ] Trend direction
- [ ] Percentage change
- [ ] Time period selected

## 5. Validate the experience (screen reader testing)

- [ ] Test with a screen reader (e.g. Narrator on Windows 11)
- [ ] Confirm the alt text reads naturally
- [ ] Verify it matches the current filter state
- [ ] Check for clarity and brevity
- [ ] Make sure it conveys the insight without referring to the visual
- [ ] Avoid repeating titles or describing colours and shapes unnecessarily
- [ ] Gather feedback from assistive technology users

## 6. Maintain and review regularly

- [ ] Revisit alt text after data refreshes
- [ ] Update it when new filters or slicers are added
- [ ] Revise it after visual redesigns
- [ ] Adjust it when the audience changes
- [ ] Review it if the report becomes customer-facing or regulated

**Review questions:**

- [ ] Does the alt text still reflect the insight?
- [ ] Would a non-visual user understand the same story as a sighted user?

## 7. Final empathy check

- [ ] Would this description help someone understand the meaning without seeing the visual?
- [ ] Does it respect the user's time and cognitive load?
- [ ] Does it communicate insight, not decoration?
- [ ] Does it reflect the visual's intended message?

---

## Related resources

- [Power BI Alt Text UDF Library](https://github.com/Juls-BI/powerbi-alttext-udfs): reusable DAX user-defined functions for dynamic alt text
- [Automating Alt Text in Power BI with DAX User-Defined Functions](https://smart-frames.co.uk/2026/03/02/automating-alt-text-in-power-bi-with-dax-user-defined-functions/), blog post
- [Power BI accessibility checklist](power-bi-accessibility-checklist.md), in this repository
