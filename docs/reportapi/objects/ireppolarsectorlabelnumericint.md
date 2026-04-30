---
title: "IRepPolarSectorLabelNumericInt"
description: "The PolarSectorNumbers object provides the font attributes for the circle numbers in a polar axis system in DIAdem REPORT."
---

# IRepPolarSectorLabelNumericInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarSectorNumbers

The PolarSectorNumbers object provides the font attributes for the circle numbers in a polar axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPolarAxisSystem.Position.ByCoordinate.X1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.Y1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.X2 = 80
oMyPolarAxisSystem.Position.ByCoordinate.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyPolarSector = oMyPolarAxisSystem.Sectors
oMyPolarSector.AutoScalingType = dd.eAxisScalingSimpleManual
oMyPolarSectorNumbers = oMyPolarSector.Numbers
oMyPolarSectorNumbers.Font.Bold = True
oMyPolarSectorNumbers.AngleUnit = dd.eAngleUnitDegree
oMyPolarSectorNumbers.Angle = 45
oMyPolarSectorNumbers.Font.Color.SetPredefinedColor(dd.eColorIndexDarkBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarsectorlabelnumericint-angle/">Angle</a> | <a href="../../properties/ireppolarsectorlabelnumericint-angleunit/">AngleUnit</a> | <a href="../../properties/ireppolarsectorlabelnumericint-displaytype/">DisplayType</a> | <a href="../../properties/ireppolarsectorlabelnumericint-font/">Font</a> | <a href="../../properties/ireppolarsectorlabelnumericint-format/">Format</a> | <a href="../../properties/ireppolarsectorlabelnumericint-relativeposition/">RelativePosition</a> | <a href="../../properties/ireppolarsectorlabelnumericint-showendlabels/">ShowEndLabels</a> | <a href="../../properties/ireppolarsectorlabelnumericint-usecurvecolor/">UseCurveColor</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarsectorsint/">PolarSectors</a>.<a href="../../properties/ireppolarsectorsint-numbers/">Numbers</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarSectorLabelNumericInt.htm`*
