---
title: "IRepImageInt.Position"
description: "Specifies the position of a graphic in a DIAdem REPORT worksheet."
---

# IRepImageInt.Position

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Position for Image

Specifies the position of a graphic in a DIAdem REPORT worksheet.

## Signature

```python
return_value = obj.Position
```

## Python example

```python
dd.Report.NewLayout()
oMyImage = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectImage, "MyImage")
oMyImage.FileName = dd.MediaLibrPath + "Example1.png"
oMyImage.BackgroundColor.SetPredefinedColor(dd.eColorIndexDarkRed)
oMyImage.Position.ByBorder.Left = 30
oMyImage.Position.ByBorder.Right = 60
oMyImage.Position.ByBorder.Top = 10
oMyImage.Position.ByBorder.Bottom = 70
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Position_IRepImageInt.htm`*
