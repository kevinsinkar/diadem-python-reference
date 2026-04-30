---
title: "IRepD3ShapeObjIsolinesSettingsInt.DisplayType"
description: "Specifies how DIAdem REPORT displays the curve of a 3D axis system in the Isolines display mode in DIAdem REPORT."
---

# IRepD3ShapeObjIsolinesSettingsInt.DisplayType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DisplayType for 3DIsolinesSettings

Specifies how DIAdem REPORT displays the curve of a 3D axis system in the Isolines display mode in DIAdem REPORT.

## Signature

```python
obj.DisplayType
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DisplayType_IRepD3ShapeObjIsolinesSettingsInt.htm`*
