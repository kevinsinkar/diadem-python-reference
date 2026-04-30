---
title: "IRepTable3DSettingsInt.Orientation"
description: "Specifies the alignment of a 3D table in DIAdem REPORT."
---

# IRepTable3DSettingsInt.Orientation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Orientation for 3DTableSettings

Specifies the alignment of a 3D table in DIAdem REPORT.

## Signature

```python
obj.Orientation
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eTableOrientationHorizontal` | 0 | Horizontal |
| `eTableOrientationVertical` | 1 | Vertical |

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
oMySettings = oMy3DTable.Settings
oMySettings.UseAutoFontSize = False
oMySettings.Orientation = dd.eTableOrientationHorizontal
oMyX = oMy3DTable.X
oMyX.Channel.Reference = "[2]/[1]"
oMyX.Font.Size = 2
oMyX.Format = "d.dd"
oMyX.Header.TitleSize = 60
oMyY = oMy3DTable.Y
oMyY.Channel.Reference = "[2]/[2]"
oMyY.Font.Size = 2
oMyY.Format = "d.dd"
oMyY.Header.TitleSize = 60
oMyZ = oMy3DTable.Z
oMyZ.Channel.Reference = "[2]/[3]"
oMyZ.Font.Size = 2
oMyZ.Format = "d.dd"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Orientation_IRepTable3DSettingsInt.htm`*
