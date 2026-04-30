---
title: "IRepSettingsImageExportTIFInt.Height"
description: "Specifies in DIAdem REPORT the height of the layout exported in a TIF format."
---

# IRepSettingsImageExportTIFInt.Height

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Height for SettingsImageExportTIF

Specifies in DIAdem REPORT the height of the layout exported in a TIF format.

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
oMyTIFExport = dd.Report.Settings.ImageExport.TIF
oMyTIFExport.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
oMyTIFExport.Height = 300
oMyTIFExport.UseCompression = False
oMyTIFExport.UseRatio = False
oMyTIFExport.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypeTIF)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Height_IRepSettingsImageExportTIFInt.htm`*
