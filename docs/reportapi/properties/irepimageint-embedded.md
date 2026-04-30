---
title: "IRepImageInt.Embedded"
description: "Specifies whether DIAdem REPORT embeds an image in a layout file."
---

# IRepImageInt.Embedded

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Embedded for Image

Specifies whether DIAdem REPORT embeds an image in a layout file.

## Signature

```python
obj.Embedded
```

## Python example

```python
dd.Report.NewLayout()
oMyImage = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectImage, "MyImage")
oMyImage.FileName = dd.MediaLibrPath + "Example1.png"
oMyImage.Position.ByCoordinate.Height = 40
oMyImage.Position.ByCoordinate.Width = 40
oMyImage.BackgroundColor.SetPredefinedColor(dd.eColorIndexDarkRed)
oMyImage.Embedded = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Embedded_IRepImageInt.htm`*
