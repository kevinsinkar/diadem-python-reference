---
title: "IRepTable2DColumnHeaderSettingsInt"
description: "The 2DTableColumnHeaderSettings object provides the header properties of a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnHeaderSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableColumnHeaderSettings

The 2DTableColumnHeaderSettings object provides the header properties of a 2D table in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMy2DTable.Settings.Header.Height = 20
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
Col2HeadSettings = oMyColumn2.Settings.Header.IndividualSettings
Col2HeadSettings.Enable = True
Col2HeadSettings.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
Col2TitleSettings = oMyColumn2.Settings.Header.IndividualTitle
Col2TitleSettings.Enable = True
Col2TitleSettings.Title1 = "Title 1"
Col2TitleSettings.Title2 = "Title 2"
Col2TitleSettings.Title3 = "Title 3"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumnheadersettingsint-individualsettings/">IndividualSettings</a> | <a href="../../properties/ireptable2dcolumnheadersettingsint-individualtitle/">IndividualTitle</a> | <a href="../../properties/ireptable2dcolumnheadersettingsint-ondrawingcell/">OnDrawingCell</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dcolumnsettingsint/">2DTableColumnSettings</a>.<a href="../../properties/ireptable2dcolumnsettingsint-header/">Header</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnHeaderSettingsInt.htm`*
