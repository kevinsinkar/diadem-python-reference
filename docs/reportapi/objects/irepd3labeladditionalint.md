---
title: "IRepD3LabelAdditionalInt"
description: "The 3DAdditionalLabel object provides the properties of the labels in a 3D axis system in DIAdem REPORT."
---

# IRepD3LabelAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DAdditionalLabel

The 3DAdditionalLabel object provides the properties of the labels in a 3D axis system in DIAdem REPORT.

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.ddde"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 8
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3labeladditionalint-angle/">Angle</a> | <a href="../../properties/irepd3labeladditionalint-font/">Font</a> | <a href="../../properties/irepd3labeladditionalint-fromchannel/">FromChannel</a> | <a href="../../properties/irepd3labeladditionalint-indexvalueformat/">IndexValueFormat</a> | <a href="../../properties/irepd3labeladditionalint-indexvaluevisible/">IndexValueVisible</a> | <a href="../../properties/irepd3labeladditionalint-position/">Position</a> | <a href="../../properties/irepd3labeladditionalint-relativeposition/">RelativePosition</a> | <a href="../../properties/irepd3labeladditionalint-repetition/">Repetition</a> | <a href="../../properties/irepd3labeladditionalint-separator/">Separator</a> | <a href="../../properties/irepd3labeladditionalint-text/">Text</a> | <a href="../../properties/irepd3labeladditionalint-textvisible/">TextVisible</a> | <a href="../../properties/irepd3labeladditionalint-visible/">Visible</a> | <a href="../../properties/irepd3labeladditionalint-xvalueformat/">XValueFormat</a> | <a href="../../properties/irepd3labeladditionalint-xvaluevisible/">XValueVisible</a> | <a href="../../properties/irepd3labeladditionalint-yvalueformat/">YValueFormat</a> | <a href="../../properties/irepd3labeladditionalint-yvaluevisible/">YValueVisible</a> | <a href="../../properties/irepd3labeladditionalint-zvalueformat/">ZValueFormat</a> | <a href="../../properties/irepd3labeladditionalint-zvaluevisible/">ZValueVisible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjbarsextensionsint/">3DBarsExtensions</a>.<a href="../../properties/irepd3shapeobjbarsextensionsint-label/">Label</a> | <a href="../irepd3shapeobjlineextensionsint/">3DLineExtensions</a>.<a href="../../properties/irepd3shapeobjlineextensionsint-label/">Label</a> | <a href="../irepd3shapeobjmatrix2dextensionsint/">3DMatrix2DExtensions</a>.<a href="../../properties/irepd3shapeobjmatrix2dextensionsint-label/">Label</a> | <a href="../irepd3shapeobjpointsextensionsint/">3DPointsExtensions</a>.<a href="../../properties/irepd3shapeobjpointsextensionsint-label/">Label</a> | <a href="../irepd3shapeobjspikeextensionsint/">3DSpikesExtensions</a>.<a href="../../properties/irepd3shapeobjspikeextensionsint-label/">Label</a> | <a href="../irepd3shapeobjsurfaceextensionsint/">3DSurfaceExtensions</a>.<a href="../../properties/irepd3shapeobjsurfaceextensionsint-label/">Label</a> | <a href="../irepd3shapeobjvectorextensionsint/">3DVectorExtensions</a>.<a href="../../properties/irepd3shapeobjvectorextensionsint-label/">Label</a> | <a href="../irepd3shapeobjwaterfallextensionsint/">3DWaterfallExtensions</a>.<a href="../../properties/irepd3shapeobjwaterfallextensionsint-label/">Label</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3LabelAdditionalInt.htm`*
