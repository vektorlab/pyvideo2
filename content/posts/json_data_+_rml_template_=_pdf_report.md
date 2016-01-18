---
Category: 'EuroPython 2011'
Copyright: 'Standard YouTube License'
Language: 'English'
SourceUrl: '"http://www.youtube.com/watch?v=9Cq_Zmr0OgM"'
ThumbnailUrl: 'http://i.ytimg.com/vi/9Cq_Zmr0OgM/hqdefault.jpg'
date: '2011-07-13'
speakers: [Stefano Cotta Ramusino]
tags: [internationalization, json, matplotlib]
---
The main problem with reports generated in Python is how to separate the
content from the style using ReportLab library, because all informations
should be saved in a single source file that, by example, is impossible to
understand for your graphic designer.

So the solution: just modularizes all components you need and identify simple
container formats for your data input (JSON) and document template (ReportLab
RML).

Now with the power of Genshi and XInclude we will create dynamic templates
that include specific snippets (e.g., to generate on the fly a decent graph
with matplotlib or cairoplot to fill some lacks of ReportLab) and we will
detach the stylesheet from the template structure.

And at the end you can also have the internationalization service in the PDF
report generation!

