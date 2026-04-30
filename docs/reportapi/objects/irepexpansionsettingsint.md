---
title: "IRepExpansionSettingsInt"
description: "The CurveExpansionSettings object provides properties of expanding curves in DIAdem REPORT."
---

# IRepExpansionSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CurveExpansionSettings

The CurveExpansionSettings object provides properties of expanding curves in DIAdem REPORT.

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
oMyShape = oMyCurve.Shape
oMyShape.Settings.UseCurveExpansion = True
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "Temp_A"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepexpansionsettingsint-attributelist/">AttributeList</a> | <a href="../../properties/irepexpansionsettingsint-enable/">Enable</a> | <a href="../../properties/irepexpansionsettingsint-mode/">Mode</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepexpansionsettingsint-collapse/">Collapse</a> | <a href="../../methods/irepexpansionsettingsint-expand/">Expand</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsettingsint/">Settings</a>.<a href="../../properties/irepsettingsint-curveexpansion/">CurveExpansion</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepExpansionSettingsInt.htm`*
