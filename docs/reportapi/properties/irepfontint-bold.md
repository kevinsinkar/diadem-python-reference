---
title: "IRepFontInt.Bold"
description: "Specifies whether DIAdem REPORT displays text in bold type."
---

# IRepFontInt.Bold

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Bold for Font

Specifies whether DIAdem REPORT displays text in bold type.

## Signature

```python
obj.Bold
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
oMyFont.Bold = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Bold_IRepFontInt.htm`*
