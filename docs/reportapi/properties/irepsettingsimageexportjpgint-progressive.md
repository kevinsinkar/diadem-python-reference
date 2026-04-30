---
title: "IRepSettingsImageExportJPGInt.Progressive"
description: "Specifies the number of steps DIAdem takes to sharpen the display of a JPEG graphic when exporting a layout as a graphic in DIAdem REPORT. The value 0 is baseli"
---

# IRepSettingsImageExportJPGInt.Progressive

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Progressive for SettingsImageExportJPG

Specifies the number of steps DIAdem takes to sharpen the display of a JPEG graphic when exporting a layout as a graphic in DIAdem REPORT. The value 0 is baseline JPEG, which older browsers and graphics programs also understand.

## Signature

```python
obj.Progressive
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyJPGExport = dd.Report.Settings.ImageExport.JPG
oMyJPGExport.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
oMyJPGExport.Height = 300
oMyJPGExport.UseRatio = True
oMyJPGExport.Width = 400
oMyJPGExport.Progressive = 5
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypeJPG)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Progressive_IRepSettingsImageExportJPGInt.htm`*
