---
title: "IRepTable3DSettingsInt.GridVertical"
description: "Specifies the vertical grid of a 3D table in DIAdem REPORT."
---

# IRepTable3DSettingsInt.GridVertical

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: GridVertical for 3DTableSettings

Specifies the vertical grid of a 3D table in DIAdem REPORT.

## Signature

```python
return_value = obj.GridVertical
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
oMy3DTable.Settings.GridHorizontal.Visible = False
oMy3DTable.Settings.GridVertical.Visible = False
oMyX = oMy3DTable.X
oMyY = oMy3DTable.Y
oMyZ = oMy3DTable.Z
oMySettings = oMy3DTable.Settings
oMySettings.UseAutoFontSize = False
oMySettings.BackgroundColor.SetPredefinedColor(dd.eColorIndexGrey )
oMyX.Channel.Reference = "[2]/[1]"
oMyX.Font.Size = 2
oMyX.Format = "d.dd"
oMyY.Channel.Reference = "[2]/[2]"
oMyY.Font.Size = 2
oMyY.Format = "d.dd"
oMyZ.Channel.Reference = "[2]/[3]"
oMyZ.Font.Size = 2
oMyZ.Format = "d.dd"
oMyX.Header.TitleSize = 60
oMyY.Header.TitleSize = 60
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_GridVertical_IRepTable3DSettingsInt.htm`*
