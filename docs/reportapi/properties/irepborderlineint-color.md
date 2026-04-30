---
title: "IRepBorderLineInt.Color"
description: "Specifies the color of a frame line in DIAdem REPORT."
---

# IRepBorderLineInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for BorderLine

Specifies the color of a frame line in DIAdem REPORT.

## Signature

```python
return_value = obj.Color
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.BorderLine.Color.SetPredefinedColor(dd.eColorIndexDarkBlue)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepBorderLineInt.htm`*
