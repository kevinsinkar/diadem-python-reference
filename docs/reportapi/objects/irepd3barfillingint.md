---
title: "IRepD3BarFillingInt"
description: "The 3DBarFilling object provides the properties of a bar display in a 3D axis system in DIAdem REPORT."
---

# IRepD3BarFillingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DBarFilling

The 3DBarFilling object provides the properties of a bar display in a 3D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem, "My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.ePredefinedColorGreen)
oMyFilling = oMySettings.Filling
oMyFilling.Enable = True
oMyFilling.EdgeColor.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3barfillingint-edgecolor/">EdgeColor</a> | <a href="../../properties/irepd3barfillingint-enable/">Enable</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjbarssettingsint/">3DBarsSettings</a>.<a href="../../properties/irepd3shapeobjbarssettingsint-filling/">Filling</a> | <a href="../irepd3shapeobjmatrix2dsettingsint/">3DMatrix2DSettings</a>.<a href="../../properties/irepd3shapeobjmatrix2dsettingsint-filling/">Filling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3BarFillingInt.htm`*
