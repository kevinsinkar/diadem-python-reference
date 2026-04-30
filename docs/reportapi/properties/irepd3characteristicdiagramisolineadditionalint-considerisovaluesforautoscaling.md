---
title: "IRepD3CharacteristicDiagramIsolineAdditionalInt.ConsiderIsoValuesForAutoScaling"
description: "Specifies whether DIAdem REPORT includes the isovalues which DIAdem takes from a data channel, the contour table, or the extended isolines when autoscaling the "
---

# IRepD3CharacteristicDiagramIsolineAdditionalInt.ConsiderIsoValuesForAutoScaling

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ConsiderIsoValuesForAutoScaling for 3DAdditionalCharacteristicDiagramIsoline

Specifies whether DIAdem REPORT includes the isovalues which DIAdem takes from a data channel, the contour table, or the extended isolines when autoscaling the axes.

## Signature

```python
obj.ConsiderIsoValuesForAutoScaling
```

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
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeCharacteristicDiagram, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.DataStructure = dd.e3DDataStructureMatrix
iChannelMax = dd.Data.Root.ChannelGroups(2).Channels(3).Properties("maximum").Value
iChannelMin = dd.Data.Root.ChannelGroups(2).Channels(3).Properties("minimum").Value
oMyIsoValTable = oMyShape.Settings.IsoValueTable
oMyIsoValTable.Count = 5
oMy3DCurve.Shape.Extensions.Isoline.Type = dd.e3DCharacteristicIsoValueFromIsoValueTable
oMy3DCurve.Shape.Extensions.Isoline.Color.ColorIndex = dd.eColorIndexPalette
oMy3DCurve.Shape.Extensions.Isoline.ConsiderIsoValuesForAutoScaling = True
for i in range( 1, oMyIsoValTable.Count+1):
    oMyIsoValTable.Item(i).Color.SetPredefinedColor(i)
    oMyIsoValTable.Item(i).Interval = 20
    oMyIsoValTable.Item(i).LineType = dd.eLineTypeDotted
    oMyIsoValTable.Item(i).UpperLimit = iChannelMin + (iChannelMax - iChannelMin) / oMyIsoValTable.Count * i
    oMyIsoValTable.Item(i).Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ConsiderIsoValuesForAutoScaling_IRepD3CharacteristicDiagramIsolineAdditionalInt.htm`*
