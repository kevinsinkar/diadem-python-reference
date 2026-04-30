---
title: "IRepTable2DSettingsInt"
description: "The 2DTableSettings object provides the properties of a 2D table in DIAdem REPORT."
---

# IRepTable2DSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableSettings

The 2DTableSettings object provides the properties of a 2D table in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMySettings = oMy2DTable.Settings
oMySettings.Header.Height = 20
oMySettings.BackgroundColor.SetPredefinedColor(dd.eColorIndexGrey)
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/ireptable2dsettingsint-borderlinecolor/">BorderLineColor</a> | <a href="../../properties/ireptable2dsettingsint-columnbackground/">ColumnBackground</a> | <a href="../../properties/ireptable2dsettingsint-columnexpansionmode/">ColumnExpansionMode</a> | <a href="../../properties/ireptable2dsettingsint-footer/">Footer</a> | <a href="../../properties/ireptable2dsettingsint-gridhorizontal/">GridHorizontal</a> | <a href="../../properties/ireptable2dsettingsint-gridvertical/">GridVertical</a> | <a href="../../properties/ireptable2dsettingsint-header/">Header</a> | <a href="../../properties/ireptable2dsettingsint-hideemptylines/">HideEmptyLines</a> | <a href="../../properties/ireptable2dsettingsint-indexsettings/">IndexSettings</a> | <a href="../../properties/ireptable2dsettingsint-orientation/">Orientation</a> | <a href="../../properties/ireptable2dsettingsint-palette/">Palette</a> | <a href="../../properties/ireptable2dsettingsint-rowbackground/">RowBackground</a> | <a href="../../properties/ireptable2dsettingsint-useautofontsize/">UseAutoFontSize</a> | <a href="../../properties/ireptable2dsettingsint-usechanneltransformation/">UseChannelTransformation</a> | <a href="../../properties/ireptable2dsettingsint-usesorting/">UseSorting</a> | <a href="../../properties/ireptable2dsettingsint-usexdoubleline/">UseXDoubleLine</a> | <a href="../../properties/ireptable2dsettingsint-useydoubleline/">UseYDoubleLine</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dint/">2DTable</a>.<a href="../../properties/ireptable2dint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DSettingsInt.htm`*
