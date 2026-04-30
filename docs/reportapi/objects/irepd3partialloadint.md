---
title: "IRepD3PartialLoadInt"
description: "The D3PartialLoad object provides the properties of partial load structures in a characteristic diagram in DIAdem REPORT."
---

# IRepD3PartialLoadInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: D3PartialLoad

The D3PartialLoad object provides the properties of partial load structures in a characteristic diagram in DIAdem REPORT.

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
oMyPartialLoad.PartialLoadToleranceType = dd.e3DPartialLoadToleranceAbsolute
oMyPartialLoad.AbsoluteTolerance = 3
oMyPartialLoad.ShowToleranceBand = True
oMyPartialLoad.MinNumberOfPoints = 5
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd3partialloadint-absolutetolerance/">AbsoluteTolerance</a> | <a href="../../properties/irepd3partialloadint-checkzvalue/">CheckZValue</a> | <a href="../../properties/irepd3partialloadint-maximumzvalue/">MaximumZValue</a> | <a href="../../properties/irepd3partialloadint-minimumzvalue/">MinimumZValue</a> | <a href="../../properties/irepd3partialloadint-minnumberofpoints/">MinNumberOfPoints</a> | <a href="../../properties/irepd3partialloadint-partialloadtolerancetype/">PartialLoadToleranceType</a> | <a href="../../properties/irepd3partialloadint-relativetolerance/">RelativeTolerance</a> | <a href="../../properties/irepd3partialloadint-showtoleranceband/">ShowToleranceBand</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd3shapeobjcharacteristicdiagramsettingsint/">3DCharacteristicDiagramSettings</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-partialload/">PartialLoad</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD3PartialLoadInt.htm`*
