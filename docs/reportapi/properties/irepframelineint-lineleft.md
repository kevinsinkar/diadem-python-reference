---
title: "IRepFrameLineInt.LineLeft"
description: "Specifies the properties of the left frame line of a comment or a rectangle in DIAdem REPORT."
---

# IRepFrameLineInt.LineLeft

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineLeft for FrameLine

Specifies the properties of the left frame line of a comment or a rectangle in DIAdem REPORT.

## Signature

```python
return_value = obj.LineLeft
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyFrameLine = oMyComment.Comment.BorderLine
oMyLineIndividual = oMyFrameLine.LineLeft
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

*Source: `ReportApi/properties/Report_property_LineLeft_IRepFrameLineInt.htm`*
