# Power BI chart selection checklist

*Data Tides · Juliana Smith*

A checklist for choosing visuals that answer the question, not just fill the page. Start with what people need to understand, then pick the chart.

---

## 1. Start with the question

- [ ] **You can state the question this visual answers in one sentence**  
  For example, "Which regions are behind target this quarter?" If you can't, the visual may not need to be there.
- [ ] **You know who will use it and what they'll do with the answer**  
  A decision-maker scanning for exceptions needs a different visual from an analyst exploring detail.
- [ ] **You've identified the type of comparison**  
  Most questions are one of these: comparison, change over time, part-to-whole, ranking, distribution, relationship, variance against a target, location or a single headline value.

## 2. Match the chart to the purpose

Use this as a starting point, not a rule book.

| Purpose | Good choices | Use with care |
|---|---|---|
| Compare categories | Bar chart (horizontal for long labels), column chart | Pie or donut, treemap |
| Change over time | Line chart, column chart for few periods | Area chart, stacked area |
| Part-to-whole | 100% stacked bar, single stacked bar | Pie or donut with more than 3–4 slices |
| Ranking | Sorted bar chart | Unsorted visuals |
| Distribution | Histogram (binned column chart), box plot | Averages on their own |
| Relationship | Scatter chart | Dual-axis charts |
| Variance against target | Bullet chart, bar with target line, variance bars | Gauges |
| Location | Filled map or map only when location matters | Maps used for decoration |
| Single value | Card or KPI visual with context (target, trend) | A number with no comparison |
| Precise values or lookup | Table or matrix | Charts with every data label switched on |

- [ ] **The chart type suits the question and the data**
- [ ] **A simpler visual wouldn't do the job just as well**  
  A sorted bar chart often beats a more complex visual. Novelty slows people down.
- [ ] **A table is used when people need exact values**  
  Charts show patterns. Tables help people look things up.

## 3. Check the data fits the chart

- [ ] **The number of categories is manageable**  
  More than 7–10 categories usually needs sorting, grouping into "Other", a Top N filter or a different visual.
- [ ] **Long category names are readable**  
  Use a horizontal bar chart instead of rotating labels on a column chart.
- [ ] **Bars are sorted in a meaningful order**  
  Sort by value for ranking, or keep a natural order for time, age bands or stages.
- [ ] **Time is shown left to right, at the right level of detail**  
  Daily data may be noise when people need a monthly trend.
- [ ] **Negative values display clearly**  
  Check the chart handles them, and that colour or labels make them obvious.
- [ ] **Too many series aren't crammed into one chart**  
  More than 4–5 lines usually becomes a tangle. Consider small multiples or highlighting one series.

## 4. Power BI specifics

- [ ] **Cards and KPI visuals show context, not just a number**  
  Add a target, previous period or trend so people know whether the number is good.
- [ ] **Custom visuals are only used when a built-in visual can't do the job**  
  Prefer certified visuals, and check they support keyboard navigation, screen readers and your organisation's policy.
- [ ] **Maps are used only when geography is part of the answer**  
  Check location data is clean and that the map doesn't expose sensitive data.
- [ ] **Gauges and decorative visuals earn their space**  
  They take a lot of room to show one value. A card or bullet chart is often clearer.
- [ ] **Small multiples are considered for comparing many groups**  
  They keep each chart simple while still showing the full picture.

## 5. Test the choice

- [ ] **Someone can answer the question within 5 seconds**  
  Show the visual to a colleague and ask what it tells them.
- [ ] **The visual doesn't repeat information shown elsewhere on the page**  
  A KPI card, a chart and a table showing the same total is clutter, not emphasis.
- [ ] **It still works on the screen size people will use**  
  Check it on a laptop, not just a large monitor, and in the mobile layout if that's used.
- [ ] **The insight can be described in alt text**  
  If you can't summarise what the visual shows, people probably can't either. See the [alt text checklist](power-bi-alt-text-checklist.md).
- [ ] **AI-suggested visuals are checked against the question**  
  AI can produce a page that looks balanced while choosing charts that don't suit the data. You decide what earns its place.

---

Next, check the chart tells the truth: [Power BI chart honesty checklist](power-bi-chart-honesty-checklist.md).
