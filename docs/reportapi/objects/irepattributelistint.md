---
title: "IRepAttributeListInt"
description: "The AttributeList object provides curve properties of expanding curves in DIAdem REPORT."
---

# IRepAttributeListInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: AttributeList

The AttributeList object provides curve properties of expanding curves in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "TR_M17_QT_32-1.tdm","TDM","")
dd.Report.NewLayout()
oMyReportSettings = dd.Report.Settings
oMyReportSettings.CurveExpansion.Enable = True
oMyReportSettings.CurveExpansion.AttributeList.Enable = True

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurve.Shape.Settings.UseCurveExpansion = True
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "Temp_A"
oMyCurveLegend = oMy2DaxisSystem.CurveLegend
oMyCurveLegend.Visible = True
oMyCurveLegend.Settings.ShowOnlyFirstCurve = True
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepattributelistint-enable/">Enable</a> | <a href="../../properties/irepattributelistint-linestyles/">LineStyles</a> | <a href="../../properties/irepattributelistint-uselinecolor/">UseLineColor</a> | <a href="../../properties/irepattributelistint-uselineinterval/">UseLineInterval</a> | <a href="../../properties/irepattributelistint-uselinetype/">UseLineType</a> | <a href="../../properties/irepattributelistint-uselinewidth/">UseLineWidth</a> | <a href="../../properties/irepattributelistint-usemarkerproperties/">UseMarkerProperties</a> | <a href="../../properties/irepattributelistint-usemarkertype/">UseMarkerType</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepexpansionsettingsint/">CurveExpansionSettings</a>.<a href="../../properties/irepexpansionsettingsint-attributelist/">AttributeList</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepAttributeListInt.htm`*
