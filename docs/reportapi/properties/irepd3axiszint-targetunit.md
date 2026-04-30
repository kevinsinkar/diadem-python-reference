---
title: "IRepD3AxisZInt.TargetUnit"
description: "Specifies the unit for the values of the z-axis in a 3D axis system in DIAdem REPORT. If you assign a value to the TargetUnit property, DIAdem converts the chan"
---

# IRepD3AxisZInt.TargetUnit

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TargetUnit for 3DAxisZ

Specifies the unit for the values of the z-axis in a 3D axis system in DIAdem REPORT. If you assign a value to the TargetUnit property, DIAdem converts the channels you want to display into this unit. If DIAdem cannot convert the unit, DIAdem does not display the data. You cannot convert the units if data for a curve entry is available in the form of a matrix.

## Signature

```python
obj.TargetUnit
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve.Shape.DataStructure = dd.e3DDataStructureTriplet
oMy3DAxisSystem.AxisList.Z.TargetUnit = "m"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TargetUnit_IRepD3AxisZInt.htm`*
