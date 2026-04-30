---
title: "IRepD2ShapeObjConstantSettingsInt"
description: "The 2DConstantSettings object provides the curve parameter properties of a 2D axis system in the Constant display mode in DIAdem REPORT."
---

# IRepD2ShapeObjConstantSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DConstantSettings

The 2DConstantSettings object provides the curve parameter properties of a 2D axis system in the Constant display mode in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurveLine = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurveLine.Shape.XChannel.Reference = "[1]/[1]"
oMyCurveLine.Shape.YChannel.Reference = "[1]/[2]"
oMyCurveConst = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeConstant, "MyConstant")
oMyCurveConst.Shape.XConstant.Reference = 10
oMyCurveConst.Shape.YConstant.Reference = 20
oMySettings = oMyCurveConst.Shape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjconstantsettingsint-line/">Line</a> | <a href="../../properties/irepd2shapeobjconstantsettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjconstantsettingsint-xfillingcolor/">XFillingColor</a> | <a href="../../properties/irepd2shapeobjconstantsettingsint-xyfillingcolor/">XYFillingColor</a> | <a href="../../properties/irepd2shapeobjconstantsettingsint-yfillingcolor/">YFillingColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjconstantint/">2DConstant</a>.<a href="../../properties/irepd2shapeobjconstantint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjConstantSettingsInt.htm`*
