---
title: "IRepSettingsImageExportJPGInt.BitsPerPixel"
description: "Specifies in DIAdem REPORT the color depth of a graphic exported in a JPG format."
---

# IRepSettingsImageExportJPGInt.BitsPerPixel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BitsPerPixel for SettingsImageExportJPG

Specifies in DIAdem REPORT the color depth of a graphic exported in a JPG format.

## Signature

```python
obj.BitsPerPixel
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eJPGBitsPerPixelRGB24YUV444` | 0 | YUV444 format for 24 bit RGB |
| `eJPGBitsPerPixelRGB24YUV422` | 1 | YUV422 format for 24 bit RGB |
| `eJPGBitsPerPixelRGB24YUV411` | 2 | YUV411 format for 24 bit RGB |
| `eJPGBitsPerPixelGray8YUV400` | 3 | YUV400 format for 256 gray shades |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
OMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
OMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyJPGExport = dd.Report.Settings.ImageExport.JPG
oMyJPGExport.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
oMyJPGExport.Height = 300
oMyJPGExport.UseRatio = True
oMyJPGExport.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypeJPG)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BitsPerPixel_IRepSettingsImageExportJPGInt.htm`*
