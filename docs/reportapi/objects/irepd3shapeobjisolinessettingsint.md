---
title: "IRepD3ShapeObjIsolinesSettingsInt"
description: "The 3DIsolinesSettings object provides the properties of the curve parameters of a 3D axis system in the Isolines display mode in DIAdem REPORT."
---

# IRepD3ShapeObjIsolinesSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DIsolinesSettings

The 3DIsolinesSettings object provides the properties of the curve parameters of a 3D axis system in the Isolines display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeIsolines, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"
oMyShape.NumberOfIsoChannels.Count = 3
oMySettings = oMyShape.Settings
oMySettings.DisplayType = dd.e3DIsolineCorrespondingToIsoValueAndProjected
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3shapeobjisolinessettingsint-displaytype/">DisplayType</a> | <a href="../../properties/irepd3shapeobjisolinessettingsint-line/">Line</a> | <a href="../../properties/irepd3shapeobjisolinessettingsint-palette/">Palette</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjisolinesint/">3DIsolines</a>.<a href="../../properties/irepd3shapeobjisolinesint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3ShapeObjIsolinesSettingsInt.htm`*
