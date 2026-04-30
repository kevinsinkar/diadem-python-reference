---
title: "IRepD3LabelIsolineAdditionalInt"
description: "The 3DAdditionalIsolineLabel object provides the properties of the isoline labels in a 3D axis system in DIAdem REPORT."
---

# IRepD3LabelIsolineAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAdditionalIsolineLabel

The 3DAdditionalIsolineLabel object provides the properties of the isoline labels in a 3D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeIsolines, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[4]/[1]"
oMyShape.YChannel.Reference = "[4]/[2]"
oMyShape.NumberOfIsoChannels.Count = 3
oMyLabel = oMyShape.Extensions.IsolineLabel
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.d"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionLength
oMyLabel.Repetition.PercentValue = 30
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3labelisolineadditionalint-angle/">Angle</a> | <a href="../../properties/irepd3labelisolineadditionalint-font/">Font</a> | <a href="../../properties/irepd3labelisolineadditionalint-fromchannel/">FromChannel</a> | <a href="../../properties/irepd3labelisolineadditionalint-indexvalueformat/">IndexValueFormat</a> | <a href="../../properties/irepd3labelisolineadditionalint-indexvaluevisible/">IndexValueVisible</a> | <a href="../../properties/irepd3labelisolineadditionalint-isovalueformat/">IsoValueFormat</a> | <a href="../../properties/irepd3labelisolineadditionalint-isovaluevisible/">IsoValueVisible</a> | <a href="../../properties/irepd3labelisolineadditionalint-position/">Position</a> | <a href="../../properties/irepd3labelisolineadditionalint-relativeposition/">RelativePosition</a> | <a href="../../properties/irepd3labelisolineadditionalint-repetition/">Repetition</a> | <a href="../../properties/irepd3labelisolineadditionalint-separator/">Separator</a> | <a href="../../properties/irepd3labelisolineadditionalint-text/">Text</a> | <a href="../../properties/irepd3labelisolineadditionalint-textvisible/">TextVisible</a> | <a href="../../properties/irepd3labelisolineadditionalint-usecurvecolor/">UseCurveColor</a> | <a href="../../properties/irepd3labelisolineadditionalint-visible/">Visible</a> | <a href="../../properties/irepd3labelisolineadditionalint-xvalueformat/">XValueFormat</a> | <a href="../../properties/irepd3labelisolineadditionalint-xvaluevisible/">XValueVisible</a> | <a href="../../properties/irepd3labelisolineadditionalint-yvalueformat/">YValueFormat</a> | <a href="../../properties/irepd3labelisolineadditionalint-yvaluevisible/">YValueVisible</a> | <a href="../../properties/irepd3labelisolineadditionalint-zvalueformat/">ZValueFormat</a> | <a href="../../properties/irepd3labelisolineadditionalint-zvaluevisible/">ZValueVisible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjisolinesextensionsint/">3DIsolinesExtensions</a>.<a href="../../properties/irepd3shapeobjisolinesextensionsint-isolinelabel/">IsolineLabel</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3LabelIsolineAdditionalInt.htm`*
