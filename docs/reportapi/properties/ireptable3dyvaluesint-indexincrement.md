---
title: "IRepTable3DYValuesInt.IndexIncrement"
description: "Specifies the step width between two successive y-values in a 3D table in DIAdem REPORT. Use the IndexIncrement property if you do not want to display all y-val"
---

# IRepTable3DYValuesInt.IndexIncrement

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IndexIncrement for 3DTableYValues

Specifies the step width between two successive y-values in a 3D table in DIAdem REPORT. Use the IndexIncrement property if you do not want to display all y-values of a data channel in a 3D table. DIAdem only includes the property IndexIncrement if you assign the value FALSE to the UseAutoIndex property.

## Signature

```python
obj.IndexIncrement
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
oMyX.UseAutoIndex = False
oMyX.Channel.Reference = "[2]/[1]"
oMyX.Font.Size = 2
oMyX.Format = "d.dd"
oMyX.IndexBegin = 1
oMyX.IndexEnd = 20
oMyX.IndexIncrement = 2
oMyY.UseAutoIndex = False
oMyY.Channel.Reference = "[2]/[2]"
oMyY.Font.Size = 2
oMyY.Format = "d.dd"
oMyY.IndexBegin = 1
oMyY.IndexEnd = 20
oMyY.IndexIncrement = 2
oMyZ.Channel.Reference = "[2]/[3]"
oMyZ.Font.Size = 2
oMyZ.Format = "d.dd"
oMyX.Header.TitleSize = 70
oMyY.Header.TitleSize = 70
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IndexIncrement_IRepTable3DYValuesInt.htm`*
