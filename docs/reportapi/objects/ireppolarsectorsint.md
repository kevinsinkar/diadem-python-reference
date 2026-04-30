---
title: "IRepPolarSectorsInt"
description: "The PolarSectors object provides the sector properties of a polar axis system in DIAdem REPORT."
---

# IRepPolarSectorsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarSectors

The PolarSectors object provides the sector properties of a polar axis system in DIAdem REPORT.

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
oMyPolarSector.SectorCount = 20
oMyPolarSector.AngleDirection = dd.eAngleDirectionClockwise
oMyPolarSector.MiniSectorCount = 10
oMyPolarSector.MiniSectorLine.LineType = dd.eLineTypeDashed1
oMyPolarSector.MiniSectorStartIndex = 2
oMyPolarSector.Numbers.Format = "d"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarsectorsint-angledirection/">AngleDirection</a> | <a href="../../properties/ireppolarsectorsint-autoscalingtype/">AutoScalingType</a> | <a href="../../properties/ireppolarsectorsint-minisectorcount/">MiniSectorCount</a> | <a href="../../properties/ireppolarsectorsint-minisectorline/">MiniSectorLine</a> | <a href="../../properties/ireppolarsectorsint-minisectorstartindex/">MiniSectorStartIndex</a> | <a href="../../properties/ireppolarsectorsint-numbers/">Numbers</a> | <a href="../../properties/ireppolarsectorsint-scalingaperture/">ScalingAperture</a> | <a href="../../properties/ireppolarsectorsint-scalingorigin/">ScalingOrigin</a> | <a href="../../properties/ireppolarsectorsint-scalingzeroangle/">ScalingZeroAngle</a> | <a href="../../properties/ireppolarsectorsint-sectorcount/">SectorCount</a> | <a href="../../properties/ireppolarsectorsint-sectorline/">SectorLine</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarint/">PolarSystem</a>.<a href="../../properties/ireppolarint-sectors/">Sectors</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarSectorsInt.htm`*
