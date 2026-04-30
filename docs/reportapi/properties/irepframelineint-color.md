---
title: "IRepFrameLineInt.Color"
description: "Specifies the color of the frame line of an object in DIAdem REPORT."
---

# IRepFrameLineInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for FrameLine

Specifies the color of the frame line of an object in DIAdem REPORT.

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

*Source: `ReportApi/properties/Report_property_Color_IRepFrameLineInt.htm`*
