---
title: "IRepTable2DColumnFooterSettingsInt"
description: "The 2DTableColumnFooterSettings object provides the footer properties of a 2D table in DIAdem REPORT."
---

# IRepTable2DColumnFooterSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableColumnFooterSettings

The 2DTableColumnFooterSettings object provides the footer properties of a 2D table in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMy2DTable.Settings.Footer.Height = 20
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[2]"
oMyCol1FooterSettings = oMyColumn1.Settings.Footer.IndividualSettings
oMyCol1FooterSettings.Enable = True
oMyCol1FooterSettings.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyCol1TitleSettings = oMyColumn1.Settings.Footer.IndividualTitle
oMyCol1TitleSettings.Enable = True
oMyCol1TitleSettings.TitleDefinition1 = dd.e2DTableTitleChnSumVisible
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumnfootersettingsint-individualsettings/">IndividualSettings</a> | <a href="../../properties/ireptable2dcolumnfootersettingsint-individualtitle/">IndividualTitle</a> | <a href="../../properties/ireptable2dcolumnfootersettingsint-ondrawingcell/">OnDrawingCell</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dcolumnsettingsint/">2DTableColumnSettings</a>.<a href="../../properties/ireptable2dcolumnsettingsint-footer/">Footer</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnFooterSettingsInt.htm`*
