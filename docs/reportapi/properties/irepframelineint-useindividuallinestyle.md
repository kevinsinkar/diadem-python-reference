---
title: "IRepFrameLineInt.UseIndividualLineStyle"
description: "Specifies whether DIAdem REPORT displays the individual frame lines in different colors, line styles, and line widths."
---

# IRepFrameLineInt.UseIndividualLineStyle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseIndividualLineStyle for FrameLine

Specifies whether DIAdem REPORT displays the individual frame lines in different colors, line styles, and line widths.

## Signature

```python
obj.UseIndividualLineStyle
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyFrameLine = oMyComment.Comment.BorderLine
oMyLineIndividual = oMyFrameLine.LineBottom
oMyFrameLine.UseIndividualLineStyle  = True
oMyLineIndividual.Color.ColorIndex = dd.eColorIndexViolet
oMyLineIndividual.LineType = dd.eLineTypeDotted
oMyLineIndividual.Width = dd.eLineWidth0140
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseIndividualLineStyle_IRepFrameLineInt.htm`*
