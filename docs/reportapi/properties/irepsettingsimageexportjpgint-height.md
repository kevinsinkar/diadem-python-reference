---
title: "IRepSettingsImageExportJPGInt.Height"
description: "Specifies the height of the layout exported in the JPG format in DIAdem REPORT."
---

# IRepSettingsImageExportJPGInt.Height

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Height for SettingsImageExportJPG

Specifies the height of the layout exported in the JPG format in DIAdem REPORT.

## Signature

```python
obj.Height
```

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
oMyJPGExport.UseRatio = False
oMyJPGExport.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypeJPG)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Height_IRepSettingsImageExportJPGInt.htm`*
