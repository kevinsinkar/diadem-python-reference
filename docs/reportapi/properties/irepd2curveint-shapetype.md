---
title: "IRepD2CurveInt.ShapeType"
description: "Specifies the display mode of a curve in a 2D axis system in DIAdem REPORT. You can use the ChangeShape for 2DCurves method to change the display mode."
---

# IRepD2CurveInt.ShapeType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShapeType for 2DCurve

Specifies the display mode of a curve in a 2D axis system in DIAdem REPORT. You can use the ChangeShape for 2DCurves method to change the display mode.

## Signature

```python
obj.ShapeType
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "MyAxisSystem")
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
dd.MsgBoxDisp(oMyCurve.ShapeType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShapeType_IRepD2CurveInt.htm`*
