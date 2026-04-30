---
title: "IRepSettingsImageExportPNGInt.Width"
description: "Specifies the width of a layout exported to the PNG format in DIAdem REPORT. DIAdem REPORT only includes the property Width if you assign the value FALSE to the"
---

# IRepSettingsImageExportPNGInt.Width

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Width for SettingsImageExportPNG

Specifies the width of a layout exported to the PNG format in DIAdem REPORT. DIAdem REPORT only includes the property Width if you assign the value FALSE to the UseRatio property.

## Signature

```python
obj.Width
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
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

*Source: `ReportApi/properties/Report_property_Width_IRepSettingsImageExportPNGInt.htm`*
