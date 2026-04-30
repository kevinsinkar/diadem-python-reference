---
title: "IRepTable3DYValuesInt.Alignment"
description: "Specifies the relative position of the y-values in 3D tables in DIAdem REPORT."
---

# IRepTable3DYValuesInt.Alignment

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Alignment for 3DTableYValues

Specifies the relative position of the y-values in 3D tables in DIAdem REPORT.

## Signature

```python
obj.Alignment
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DTable,"My2DTable")
oMyPosition = oMy3DTable.Position.ByBorder
oMyPosition.Top = 20
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 20
oMyX = oMy3DTable.X
oMyY = oMy3DTable.Y
oMyZ = oMy3DTable.Z
oMySettings = oMy3DTable.Settings
oMySettings.UseAutoFontSize = False
oMyX.Channel.Reference = "[2]/[1]"
oMyX.Font.Size = 2
oMyX.Format = "d.dd"
oMyX.Alignment = dd.eTableAlignmentCentric
oMyX.Header.TitleSize = 70
oMyY.Channel.Reference = "[2]/[2]"
oMyY.Font.Size = 2
oMyY.Format = "d.dd"
oMyY.Alignment = dd.eTableAlignmentLeft
oMyY.Header.TitleSize = 70
oMyZ.Channel.Reference = "[2]/[3]"
oMyZ.Font.Size = 2
oMyZ.Format = "d.dd"
oMyZ.Alignment = dd.eTableAlignmentRight
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Alignment_IRepTable3DYValuesInt.htm`*
