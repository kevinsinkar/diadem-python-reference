---
title: "IRepPolarLabelAdditionalInt"
description: "The PolarAdditionalLabel object provides the properties of the labels of a polar curve in the display type Line and Points in DIAdem REPORT."
---

# IRepPolarLabelAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarAdditionalLabel

The PolarAdditionalLabel object provides the properties of the labels of a polar curve in the display type Line and Points in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyLabel = oMyCurve.Shape.Extensions.Label
oMyLabel.YValueVisible = True
oMyLabel.YValueFormat = "d.dd"
oMyLabel.Font.Name = "Arial"
oMyLabel.RelativePosition = dd.eRelativePositionPointCenter
oMyLabel.Repetition.Mode = dd.eLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 10
oMyLabel.Angle = 45
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarlabeladditionalint-angle/">Angle</a> | <a href="../../properties/ireppolarlabeladditionalint-font/">Font</a> | <a href="../../properties/ireppolarlabeladditionalint-fromchannel/">FromChannel</a> | <a href="../../properties/ireppolarlabeladditionalint-indexvalueformat/">IndexValueFormat</a> | <a href="../../properties/ireppolarlabeladditionalint-indexvaluevisible/">IndexValueVisible</a> | <a href="../../properties/ireppolarlabeladditionalint-relativeposition/">RelativePosition</a> | <a href="../../properties/ireppolarlabeladditionalint-repetition/">Repetition</a> | <a href="../../properties/ireppolarlabeladditionalint-separator/">Separator</a> | <a href="../../properties/ireppolarlabeladditionalint-text/">Text</a> | <a href="../../properties/ireppolarlabeladditionalint-textvisible/">TextVisible</a> | <a href="../../properties/ireppolarlabeladditionalint-xvalueformat/">XValueFormat</a> | <a href="../../properties/ireppolarlabeladditionalint-xvaluevisible/">XValueVisible</a> | <a href="../../properties/ireppolarlabeladditionalint-yvalueformat/">YValueFormat</a> | <a href="../../properties/ireppolarlabeladditionalint-yvaluevisible/">YValueVisible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarshapeobjlineandpointsextensionsint/">PolarLineAndPointsExtensions</a>.<a href="../../properties/ireppolarshapeobjlineandpointsextensionsint-label/">Label</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarLabelAdditionalInt.htm`*
