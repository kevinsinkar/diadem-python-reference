---
title: "IRepD2AxisYInt.Height"
description: "Specifies the height of the y-subaxis in relation to the first y-axis as a percentage of the length of the original axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisYInt.Height

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Height for 2DAxisY

Specifies the height of the y-subaxis in relation to the first y-axis as a percentage of the length of the original axis in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Height
```

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve1 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyFirstCurve")
oMy2DCurve1.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve1.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve2 = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MySecondCurve")
oMy2DCurve2.Shape.XChannel.Reference = "[1]/[3]"
oMy2DCurve2.Shape.YChannel.Reference = "[1]/[4]"
oMyAxis = oMy2DaxisSystem.YAxisList.Add("SecondAxis")
oMyAxis.Height = 50
oMy2DCurve2.YAxisReference = "SecondAxis"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Height_IRepD2AxisYInt.htm`*
