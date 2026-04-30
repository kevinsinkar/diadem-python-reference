---
title: "IRepSettingsImageExportPNGInt.BitsPerPixel"
description: "Specifies in DIAdem REPORT the color depth of the graphic exported in a PNG format."
---

# IRepSettingsImageExportPNGInt.BitsPerPixel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BitsPerPixel for SettingsImageExportPNG

Specifies in DIAdem REPORT the color depth of the graphic exported in a PNG format.

## Signature

```python
obj.BitsPerPixel
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePNGBitsPerPixelRGB01` | 0 | Black/White |
| `ePNGBitsPerPixelRGB04` | 1 | 16 colors |
| `ePNGBitsPerPixelRGB08` | 2 | 256 colors |
| `ePNGBitsPerPixelRGB24` | 3 | 24 bit RGB |
| `ePNGBitsPerPixelRGB32` | 4 | 32 bit RGB |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
OMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
OMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyPNGExport = dd.Report.Settings.ImageExport.PNG
oMyPNGExport.BitsPerPixel = dd.ePNGBitsPerPixelRGB32
oMyPNGExport.Height = 300
oMyPNGExport.UseRatio = True
oMyPNGExport.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypePNG)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BitsPerPixel_IRepSettingsImageExportPNGInt.htm`*
