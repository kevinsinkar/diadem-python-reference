---
title: "IRepFontInt.Size"
description: "Specifies the font size of a text as a percentage of the page height in DIAdem REPORT. DIAdem only includes the Size property in the ColorLegendSettings , Curve"
---

# IRepFontInt.Size

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Size for Font

Specifies the font size of a text as a percentage of the page height in DIAdem REPORT. DIAdem only includes the Size property in the ColorLegendSettings , CurveLegendSettings , CurveLegendHeader , ColorLegendHeader , 2DTableHeaderDefaultSettings , 2DTableSettings , and 3DTableSettings objects if you assign the value False to the UseAutoFontSize property.

## Signature

```python
obj.Size
```

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"
oMyFont = oMyComment.Comment.Font
oMyFont.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFont.Name = "Tahoma"
oMyFont.Size = 7
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Size_IRepFontInt.htm`*
