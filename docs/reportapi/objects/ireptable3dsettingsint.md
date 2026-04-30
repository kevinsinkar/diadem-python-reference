---
title: "IRepTable3DSettingsInt"
description: "The 3DTableSettings object provides the properties of a 3D table in DIAdem REPORT."
---

# IRepTable3DSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 3DTableSettings

The 3DTableSettings object provides the properties of a 3D table in DIAdem REPORT.

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
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable3dsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/ireptable3dsettingsint-gridhorizontal/">GridHorizontal</a> | <a href="../../properties/ireptable3dsettingsint-gridvertical/">GridVertical</a> | <a href="../../properties/ireptable3dsettingsint-hidezerovalues/">HideZeroValues</a> | <a href="../../properties/ireptable3dsettingsint-linecolor/">LineColor</a> | <a href="../../properties/ireptable3dsettingsint-orientation/">Orientation</a> | <a href="../../properties/ireptable3dsettingsint-useautofontsize/">UseAutoFontSize</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable3dint/">3DTable</a>.<a href="../../properties/ireptable3dint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable3DSettingsInt.htm`*
