---
title: "IRepD3ShapeObjWaterfallExtensionsInt.Spike"
description: "Specifies the properties of the additional spike display in a 3D axis system with a waterfall display in DIAdem REPORT."
---

# IRepD3ShapeObjWaterfallExtensionsInt.Spike

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Spike for 3DWaterfallExtensions

Specifies the properties of the additional spike display in a 3D axis system with a waterfall display in DIAdem REPORT.

## Signature

```python
return_value = obj.Spike
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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeWaterfall, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySpike = oMyShape.Extensions.Spike
oMySpike.Visible = True
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

*Source: `ReportApi/properties/Report_property_Spike_IRepD3ShapeObjWaterfallExtensionsInt.htm`*
