---
title: "IRepD3CharacteristicDiagramIsolineAdditionalInt.Channel"
description: "Specifies the isolines channel in a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT."
---

# IRepD3CharacteristicDiagramIsolineAdditionalInt.Channel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Channel for 3DAdditionalCharacteristicDiagramIsoline

Specifies the isolines channel in a 3D axis system in the Characteristic diagram display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Channel
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
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
oMy3DCurve.Shape.Extensions.Isoline.Type = dd.e3DCharacteristicIsoValueFromChannel
oMy3DCurve.Shape.Extensions.Isoline.Channel.Reference = "[2]/[1]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Channel_IRepD3CharacteristicDiagramIsolineAdditionalInt.htm`*
