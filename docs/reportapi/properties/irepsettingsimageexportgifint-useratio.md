---
title: "IRepSettingsImageExportGIFInt.UseRatio"
description: "Specifies whether DIAdem REPORT keeps the aspect ratio when exporting a layout into a GIF file."
---

# IRepSettingsImageExportGIFInt.UseRatio

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseRatio for SettingsImageExportGIF

Specifies whether DIAdem REPORT keeps the aspect ratio when exporting a layout into a GIF file.

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
dd.Report.Settings.ImageExport.GIF.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
dd.Report.Settings.ImageExport.GIF.Height = 300
dd.Report.Settings.ImageExport.GIF.UseRatio = True
dd.Report.Settings.ImageExport.GIF.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyNew2DCurve", dd.eImageExportTypeGIF)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseRatio_IRepSettingsImageExportGIFInt.htm`*
