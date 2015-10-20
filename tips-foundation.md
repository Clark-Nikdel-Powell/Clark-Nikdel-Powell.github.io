---
layout: page
title: Foundation Tips
excerpt: Markup gotchas to watch out for.
permalink: /tips/foundation/
status: draft
revisioncount: 1
lastedit: 10/20/15
initial: JHN
---

### Markup Notes

#### Only use rows with columns

If you nest a `.row` class within another row, Foundation applies the CSS `margin: 0 -0.9375rem;` to offset the column padding-left and right applied to a `.column`. If your horizontal alignments are off, that's likely why.