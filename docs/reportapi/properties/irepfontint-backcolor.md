---
title: "IRepFontInt.BackColor"
description: "Specifies the background color of a text in DIAdem REPORT."
---

# IRepFontInt.BackColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackColor for Font

Specifies the background color of a text in DIAdem REPORT.

## Signature

```python
return_value = obj.BackColor
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
oMyFont.BackColor.ColorIndex = dd.eColorIndexYellow
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackColor_IRepFontInt.htm`*
