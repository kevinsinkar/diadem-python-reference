---
title: "IRepAxisTickInt.Channel"
description: "Specifies the tick channel of a 3D axis system or of a polar axis system in DIAdem REPORT."
---

# IRepAxisTickInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for AxisTickObject

Specifies the tick channel of a 3D axis system or of a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Channel
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem, "My3DAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMyAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyXScaling = oMyAxisSystem.AxisList.X.Scaling
oMyXScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyXScaling.Type = dd.e3DScalingLinear
oMyTick = oMyXScaling.Tick
oMyTick.SpacingType = dd.eAxisTickSpacingReadFromChannel
oMyTick.Distance = 0.5
oMyTick.Channel.Reference = "[5]/[1]"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Channel_IRepAxisTickInt.htm`*
