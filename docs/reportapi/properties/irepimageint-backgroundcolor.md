---
title: "IRepImageInt.BackgroundColor"
description: "Specifies the background color of a graphic in DIAdem REPORT."
---

# IRepImageInt.BackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundColor for Image

Specifies the background color of a graphic in DIAdem REPORT.

## Signature

```python
return_value = obj.BackgroundColor
```

## Python example

```python
dd.Report.NewLayout()
oMyImage = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectImage, "MyImage")
oMyImage.FileName = dd.MediaLibrPath + "Example1.png"
oMyImage.Position.ByCoordinate.Height = 40
oMyImage.Position.ByCoordinate.Width = 40
oMyImage.BackgroundColor.SetPredefinedColor(dd.eColorIndexDarkRed)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundColor_IRepImageInt.htm`*
