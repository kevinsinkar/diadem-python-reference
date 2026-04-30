---
title: "IRepSettingsImageExportPNGInt.UseRatio"
description: "Specifies whether DIAdem REPORT keeps the aspect ratio when exporting a layout into a PNG file."
---

# IRepSettingsImageExportPNGInt.UseRatio

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseRatio for SettingsImageExportPNG

Specifies whether DIAdem REPORT keeps the aspect ratio when exporting a layout into a PNG file.

## Signature

```python
obj.UseRatio
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 10
oMyPos.X2 = 60
oMyPos.Y1 = 10
oMyPos.Y2 = 60
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyPNGExport = dd.Report.Settings.ImageExport.PNG
oMyPNGExport.BitsPerPixel = dd.ePNGBitsPerPixelRGB32
oMyPNGExport.Height = 300
oMyPNGExport.UseRatio = False
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

*Source: `ReportApi/properties/Report_property_UseRatio_IRepSettingsImageExportPNGInt.htm`*
