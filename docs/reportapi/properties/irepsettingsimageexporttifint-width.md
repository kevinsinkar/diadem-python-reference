---
title: "IRepSettingsImageExportTIFInt.Width"
description: "Specifies the width of a layout exported to the TIF format in DIAdem REPORT. DIAdem REPORT only includes the property Width if you assign the value FALSE to the"
---

# IRepSettingsImageExportTIFInt.Width

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Width for SettingsImageExportTIF

Specifies the width of a layout exported to the TIF format in DIAdem REPORT. DIAdem REPORT only includes the property Width if you assign the value FALSE to the UseRatio property.

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
oMyTIFExport = dd.Report.Settings.ImageExport.TIF
oMyTIFExport.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
oMyTIFExport.Height = 300
oMyTIFExport.UseCompression = False
oMyTIFExport.UseRatio = False
oMyTIFExport.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypeTIF)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Width_IRepSettingsImageExportTIFInt.htm`*
