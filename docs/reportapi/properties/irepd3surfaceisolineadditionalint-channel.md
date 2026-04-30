---
title: "IRepD3SurfaceIsolineAdditionalInt.Channel"
description: "Specifies the channel of the additional isolines in 3D axis systems in the Surface display mode in DIAdem REPORT."
---

# IRepD3SurfaceIsolineAdditionalInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for 3DAdditionalSurfaceIsoline

Specifies the channel of the additional isolines in 3D axis systems in the Surface display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Channel
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
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySurfaceIsoline = oMyShape.Extensions.SurfaceIsoline
oMySurfaceIsoline.Visible = True
oMySurfaceIsoline.Line.Color.SetPredefinedColor(dd.ePredefinedColorBlue)
oMySurfaceIsoline.Channel.Reference = "[2]/[3]"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Channel_IRepD3SurfaceIsolineAdditionalInt.htm`*
