---
title: "IRepD3SpikesAdditionalInt.Color"
description: "Specifies the color of the additional spikes display in 3D axis systems in DIAdem REPORT. Use the Visible property to enable additional spikes."
---

# IRepD3SpikesAdditionalInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for 3DAdditionalSpikes

Specifies the color of the additional spikes display in 3D axis systems in DIAdem REPORT. Use the Visible property to enable additional spikes.

## Signature

```python
return_value = obj.Color
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
oMySpike.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySpike.Width = dd.eLineWidth0100
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepD3SpikesAdditionalInt.htm`*
