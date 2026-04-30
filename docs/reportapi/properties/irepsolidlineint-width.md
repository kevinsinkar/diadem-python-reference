---
title: "IRepSolidLineInt.Width"
description: "Specifies the line width of a line in DIAdem REPORT. DIAdem REPORT only includes the Width property in the 2DAxisSettings object if you assign the value TRUE to"
---

# IRepSolidLineInt.Width

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Width for SolidLine

Specifies the line width of a line in DIAdem REPORT. DIAdem REPORT only includes the Width property in the 2DAxisSettings object if you assign the value TRUE to the UseIndividualAxisStyle property.

## Signature

```python
obj.Width
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLineWidthMin` | 0 | Minimum |
| `eLineWidth0025` | 1 | 0.25 |
| `eLineWidth0035` | 2 | 0.35 |
| `eLineWidth0050` | 3 | 0.5 |
| `eLineWidth0070` | 4 | 0.7 |
| `eLineWidth0100` | 5 | 1.0 |
| `eLineWidth0140` | 6 | 1.4 |
| `eLineWidth0200` | 7 | 2.0 |
| `eLineWidth0280` | 8 | 2.8 |
| `eLineWidth0400` | 9 | 4.0 |
| `eLineWidth0560` | 10 | 5.6 |
| `eLineWidth0800` | 11 | 8.0 |
| `eLineWidth1120` | 12 | 11.2 |
| `eLineWidth1600` | 13 | 16.0 |
| `eLineWidth2240` | 14 | 22.4 |
| `eLineWidth3200` | 15 | 32.0 |

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
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve.Shape.DataStructure = dd.e3DDataStructureMatrix
oMyXLabel = oMy3DAxisSystem.AxisList.X.Label
oMyXLabel.Text = "This is the x-axis"
oMyXLabel.Font.Name = "Tahoma"
oMyXLabel.Font.Size = 5
oMy3DAxisSystem.AxisList.X.Line.Width = dd.eLineWidth0140
oMyYLabel = oMy3DAxisSystem.AxisList.Y.Label
oMyYLabel.Text = "This is the y-axis"
oMyYLabel.Font.Name = "Tahoma"
oMyYLabel.Font.Size = 5
oMy3DAxisSystem.AxisList.Y.Line.Width = dd.eLineWidth0140
oMyZLabel = oMy3DAxisSystem.AxisList.Z.Label
oMyZLabel.Text = "This is the z-axis"
oMyZLabel.Font.Name = "Tahoma"
oMyZLabel.Font.Size = 5
oMy3DAxisSystem.AxisList.Z.Line.Width = dd.eLineWidth0050
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Width_IRepSolidLineInt.htm`*
