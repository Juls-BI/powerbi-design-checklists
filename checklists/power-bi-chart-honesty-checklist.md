# Power BI chart honesty checklist

*Data Tides · Juliana Smith*

A checklist for making sure a visual gives an honest impression of the data. A chart can be the right type and still mislead through its scale, time period, aggregation or wording.

---

## 1. Axes and scales

- [ ] **Bar and column charts start at zero**  
  Bar length represents the value, so a truncated axis exaggerates differences. Power BI sets the start automatically in some cases, so check the Y-axis range.
- [ ] **Line charts that don't start at zero make it clear**  
  Line charts can zoom in to show change, but the axis labels should make the range obvious.
- [ ] **Charts that will be compared use the same scale**  
  Small multiples and side-by-side visuals with different axis ranges suggest similar values when they're not.
- [ ] **Dual-axis charts are avoided, or both axes are clearly labelled**  
  Two scales on one chart can create relationships that aren't there. Two separate charts are usually clearer.
- [ ] **Logarithmic scales are labelled and explained**  
  Most readers assume a linear scale.
- [ ] **Intervals on the time axis are even**  
  Missing months or uneven gaps distort trends. Use a continuous date axis where it makes sense.

## 2. Time and context

- [ ] **The time period isn't chosen to tell a particular story**  
  Check whether a longer or different period would change the message.
- [ ] **Incomplete periods are flagged or excluded**  
  A current month with 10 days of data will look like a drop next to full months.
- [ ] **Comparisons are like-for-like**  
  Compare the same number of days, the same stores or the same scope, and say so.
- [ ] **Targets, benchmarks or previous periods give context**  
  A number on its own doesn't tell people whether it's good, bad or normal.
- [ ] **The data refresh date is visible**  
  People should know how current the data is.

## 3. Proportions and area

- [ ] **Part-to-whole visuals add up to 100%**  
  Check pie, donut and 100% stacked charts don't include overlapping categories.
- [ ] **No 3D effects are used**  
  3D distorts size and angle, so values in front look bigger than those behind.
- [ ] **Bubble sizes are scaled by area, not diameter**  
  Check the size field represents what you think it does.
- [ ] **Stacked charts are only used when the total matters**  
  Only the bottom segment shares a common baseline, so the middle segments are hard to compare.

## 4. Aggregation and data

- [ ] **The right aggregation is used**  
  Check whether sum, average, median or count gives an honest picture. An average can hide outliers or a skewed distribution.
- [ ] **Matrix and table totals are correct**  
  Totals in Power BI are recalculated in the total's filter context, not summed from the rows. Check they show what people expect.
- [ ] **Percentages say what they're a percentage of**  
  "20%" of the region, of the total or of last year are very different statements.
- [ ] **Blanks and zeros are treated correctly**  
  A missing value isn't the same as zero. Check how the visual and measures handle both.
- [ ] **Small numbers are flagged**  
  A 50% increase from 2 to 3 isn't the same as one from 2,000 to 3,000.
- [ ] **Active filters are visible**  
  If a visual is filtered (by a slicer, page filter or visual-level filter), people should be able to see that.
- [ ] **Outliers are explained, not silently removed**  
  If you exclude data, say what and why.

## 5. Colour and emphasis

- [ ] **Colour meaning matches the data**  
  Use sequential colours for low to high, diverging colours around a meaningful midpoint, and categorical colours for groups.
- [ ] **Good and bad colours are applied the right way round**  
  For some measures, like costs or delays, an increase is bad. Check conditional formatting reflects that.
- [ ] **Highlighting draws attention to the right thing**  
  Emphasis should point to what matters, not to the result you hope people see.

## 6. Titles, labels and wording

- [ ] **Titles describe what the data shows without overclaiming**  
  "Sales rose 12% in Q3" is a fact. "Campaign drove sales growth" is a claim that needs evidence.
- [ ] **Correlation isn't presented as cause**  
  Two lines moving together don't prove that one caused the other.
- [ ] **Units, currency and time periods are stated**  
  Make sure people know whether values are in thousands, millions, which currency and which period.
- [ ] **Data sources and definitions are available**  
  Add a note, tooltip or info page explaining how key measures are calculated.

## 7. Generated text and interpretation

- [ ] **Dynamic titles, summaries and alt text describe the direction of change correctly**  
  For example, a milestone date moving later is a delay, not an improvement. Check what the text says, not just that the DAX runs.
- [ ] **Generated text is tested across different filter selections**  
  Make sure the description still matches the visual for every combination people are likely to use.
- [ ] **AI-generated insights are checked against the data**  
  Once AI starts interpreting the data, that interpretation becomes part of what you're responsible for.

---

Start by choosing the right visual: [Power BI chart selection checklist](power-bi-chart-selection-checklist.md).
