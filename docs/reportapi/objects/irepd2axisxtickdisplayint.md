---
title: "IRepD2AxisXTickDisplayInt"
description: "The 2DAxisXTickDisplay object provides the tick properties of the x-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisXTickDisplayInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisXTickDisplay

The 2DAxisXTickDisplay object provides the tick properties of the x-axis in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DAxisSystem.Settings.UseIndividualAxisStyle = True
oMyXTickDisplay = oMy2DAxisSystem.XAxis.TickDisplay
oMyXTickDisplay.UseAutoSize = False
oMyXTickDisplay.Size = 5
oMyXTickDisplay.Type = dd.e2DAxisXTickBothSides
oMyYTickDisplay = oMy2DAxisSystem.YAxis.TickDisplay
oMyYTickDisplay.UseAutoSize = False
oMyYTickDisplay.Size = 5
oMyYTickDisplay.Type = dd.e2DAxisXTickBothSides
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2axisxtickdisplayint-size/">Size</a> | <a href="../../properties/irepd2axisxtickdisplayint-type/">Type</a> | <a href="../../properties/irepd2axisxtickdisplayint-useautosize/">UseAutoSize</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisxint/">2DAxisX</a>.<a href="../../properties/irepd2axisxint-tickdisplay/">TickDisplay</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisXTickDisplayInt.htm`*
