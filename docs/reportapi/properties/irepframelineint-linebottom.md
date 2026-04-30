---
title: "IRepFrameLineInt.LineBottom"
description: "Specifies the properties of the bottom frame line of a comment or a rectangle in DIAdem REPORT."
---

# IRepFrameLineInt.LineBottom

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineBottom for FrameLine

Specifies the properties of the bottom frame line of a comment or a rectangle in DIAdem REPORT.

## Signature

```python
return_value = obj.LineBottom
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

*Source: `ReportApi/properties/Report_property_LineBottom_IRepFrameLineInt.htm`*
