---
title: "IRepD3CurveInt.ShapeType"
description: "Specifies the display mode of a curve in a 3D axis system in DIAdem REPORT. You can use the ChangeShape for 3DCurves method to change the display mode."
---

# IRepD3CurveInt.ShapeType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShapeType for 3DCurve

Specifies the display mode of a curve in a 3D axis system in DIAdem REPORT. You can use the ChangeShape for 3DCurves method to change the display mode.

## Signature

```python
obj.ShapeType
```

## Python example

```python
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem, "MyAxisSystem")
oMyCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSpikes, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.ZChannel.Reference = "[1]/[3]"
dd.MsgBoxDisp(oMyCurve.ShapeType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShapeType_IRepD3CurveInt.htm`*
