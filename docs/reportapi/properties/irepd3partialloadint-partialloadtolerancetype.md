---
title: "IRepD3PartialLoadInt.PartialLoadToleranceType"
description: "Specifies whether you define the tolerance as a percentage of the entire x-area or as the absolute x-area, in a characteristic diagram with partial load structu"
---

# IRepD3PartialLoadInt.PartialLoadToleranceType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: PartialLoadToleranceType for D3PartialLoad

Specifies whether you define the tolerance as a percentage of the entire x-area or as the absolute x-area, in a characteristic diagram with partial load structure in DIAdem REPORT. Points whose x-values lie outside the tolerance are invalid values of the partial load.

## Signature

```python
obj.PartialLoadToleranceType
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
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyShape.TripletStructure = dd.e3DCharacteristicTripletStructurePartialLoad
oMyPartialLoad = oMyShape.Settings.PartialLoad
oMyPartialLoad.PartialLoadToleranceType = dd.e3DPartialLoadToleranceRelative
oMyPartialLoad.RelativeTolerance = 3
oMyPartialLoad.ShowToleranceBand = True
oMyPartialLoad.MinNumberOfPoints = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_PartialLoadToleranceType_IRepD3PartialLoadInt.htm`*
