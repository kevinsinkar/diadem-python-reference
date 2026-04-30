---
title: "IRepD2ShapeObjLineSettingsInt.ConnectNoValueNeighbors"
description: "Specifies whether DIAdem REPORT connects NoValues in curves in the Line display mode in a 2D axis system."
---

# IRepD2ShapeObjLineSettingsInt.ConnectNoValueNeighbors

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ConnectNoValueNeighbors for 2DLineSettings

Specifies whether DIAdem REPORT connects NoValues in curves in the Line display mode in a 2D axis system.

## Signature

```python
obj.ConnectNoValueNeighbors
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve1 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve1")
oMyShape1 = oMyCurve1.Shape
oMyShape1.XChannel.Reference = ""
oMyShape1.YChannel.Reference = "[4]/[1]"
oMyCurve1.Shape.Settings.UseCurveSmoothing = False
oMyCurve1.Shape.Settings.ConnectNoValueNeighbors = True
oMyCurve2 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve2")
oMyShape2 = oMyCurve2.Shape
oMyShape2.XChannel.Reference = ""
oMyShape2.YChannel.Reference = "[4]/[1]"
oMyCurve2.Shape.Settings.UseCurveSmoothing = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ConnectNoValueNeighbors_IRepD2ShapeObjLineSettingsInt.htm`*
