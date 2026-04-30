---
title: "IRepD3SpikesAdditionalInt.Interval"
description: "Specifies the line interval for broken lines in a display with additional spikes in a 3D axis system in DIAdem REPORT. Greater values mean greater intervals."
---

# IRepD3SpikesAdditionalInt.Interval

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Interval for 3DAdditionalSpikes

Specifies the line interval for broken lines in a display with additional spikes in a 3D axis system in DIAdem REPORT. Greater values mean greater intervals.

## Signature

```python
obj.Interval
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySpike = oMyShape.Extensions.Spike
oMySpike.Visible = True
oMySpike.LineType = dd.eLineTypeDashDot
oMySpike.Interval = 3
oMySpike.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySpike.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Interval_IRepD3SpikesAdditionalInt.htm`*
