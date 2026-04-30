---
title: "IRepD2ShapeObjSpecialCombinationSettingsInt"
description: "The 2DSpecialCombinationSettings object provides the curve parameter properties of a 2D axis system in the Special combination display mode in DIAdem REPORT."
---

# IRepD2ShapeObjSpecialCombinationSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DSpecialCombinationSettings

The 2DSpecialCombinationSettings object provides the curve parameter properties of a 2D axis system in the Special combination display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeSpecialCombination, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySetting = oMyShape.Settings
oMySetting.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySetting.Line.Width = dd.eLineWidth0100
oMyMarker = oMyShape.Extensions.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 3
oMyMarker.Repetition.Mode = dd.eMarkerRepetitionMaximalNPoints
oMyMarker.Repetition.NValue = 20
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjspecialcombinationsettingsint-connectnovalueneighbors/">ConnectNoValueNeighbors</a> | <a href="../../properties/irepd2shapeobjspecialcombinationsettingsint-filleffects/">FillEffects</a> | <a href="../../properties/irepd2shapeobjspecialcombinationsettingsint-line/">Line</a> | <a href="../../properties/irepd2shapeobjspecialcombinationsettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjspecialcombinationsettingsint-usecurveexpansion/">UseCurveExpansion</a> | <a href="../../properties/irepd2shapeobjspecialcombinationsettingsint-usecurvesmoothing/">UseCurveSmoothing</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjspecialcombinationint/">2DSpecialCombination</a>.<a href="../../properties/irepd2shapeobjspecialcombinationint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjSpecialCombinationSettingsInt.htm`*
