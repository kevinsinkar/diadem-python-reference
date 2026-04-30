---
title: "IRepTable3DSettingsInt.HideZeroValues"
description: "Specifies whether DIAdem REPORT suppresses the display of z-values in the 3D table if the z-values contain the value zero."
---

# IRepTable3DSettingsInt.HideZeroValues

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: HideZeroValues for 3DTableSettings

Specifies whether DIAdem REPORT suppresses the display of z-values in the 3D table if the z-values contain the value zero.

## Signature

```python
obj.HideZeroValues
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
oMy3DTable.Settings.HideZeroValues = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_HideZeroValues_IRepTable3DSettingsInt.htm`*
