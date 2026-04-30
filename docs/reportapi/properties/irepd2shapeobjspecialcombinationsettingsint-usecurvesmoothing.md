---
title: "IRepD2ShapeObjSpecialCombinationSettingsInt.UseCurveSmoothing"
description: "Specifies whether DIAdem REPORT smoothes the curve between two data points of a 2D curve in the Special combination display mode."
---

# IRepD2ShapeObjSpecialCombinationSettingsInt.UseCurveSmoothing

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseCurveSmoothing for 2DSpecialCombinationSettings

Specifies whether DIAdem REPORT smoothes the curve between two data points of a 2D curve in the Special combination display mode.

## Signature

```python
obj.UseCurveSmoothing
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "\\examples\\data\\Report_EXPL","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve1 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve1")
oMyCurve1.Shape.XChannel.Reference = "[6]/[1]"
oMyCurve1.Shape.YChannel.Reference = "[6]/[2]"
oMyCurve1.Shape.Settings.UseCurveSmoothing = True
oMyCurve2 = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve2")
oMyCurve2.Shape.XChannel.Reference = "[6]/[1]"
oMyCurve2.Shape.YChannel.Reference = "[6]/[2]"
oMyCurve2.Shape.Settings.UseCurveSmoothing = False
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseCurveSmoothing_IRepD2ShapeObjSpecialCombinationSettingsInt.htm`*
