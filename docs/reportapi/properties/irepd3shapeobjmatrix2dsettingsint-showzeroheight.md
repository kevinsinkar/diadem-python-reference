---
title: "IRepD3ShapeObjMatrix2DSettingsInt.ShowZeroHeight"
description: "Specifies whether DIAdem REPORT displays bars with a height of 0 in a matrix display in a 3D axis system."
---

# IRepD3ShapeObjMatrix2DSettingsInt.ShowZeroHeight

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowZeroHeight for 3DMatrix2DSettings

Specifies whether DIAdem REPORT displays bars with a height of 0 in a matrix display in a 3D axis system.

## Signature

```python
obj.ShowZeroHeight
```

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeMatrix2D, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.ShowZeroHeight = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowZeroHeight_IRepD3ShapeObjMatrix2DSettingsInt.htm`*
