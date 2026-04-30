---
title: "IRepFontInt.Italic"
description: "Specifies whether DIAdem REPORT displays text in italics."
---

# IRepFontInt.Italic

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Italic for Font

Specifies whether DIAdem REPORT displays text in italics.

## Signature

```python
obj.Italic
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
oMyFont.Italic = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Italic_IRepFontInt.htm`*
