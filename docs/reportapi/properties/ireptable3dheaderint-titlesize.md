---
title: "IRepTable3DHeaderInt.TitleSize"
description: "Specifies the ratio of the text part of the label area to the total heading area in a 3D table in DIAdem REPORT as a percentage."
---

# IRepTable3DHeaderInt.TitleSize

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TitleSize for 3DTableHeader

Specifies the ratio of the text part of the label area to the total heading area in a 3D table in DIAdem REPORT as a percentage.

## Signature

```python
obj.TitleSize
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
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
oMyY.Channel.Reference = "[2]/[2]"
oMyY.Font.Size = 2
oMyY.Format = "d.dd"
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

*Source: `ReportApi/properties/Report_property_TitleSize_IRepTable3DHeaderInt.htm`*
