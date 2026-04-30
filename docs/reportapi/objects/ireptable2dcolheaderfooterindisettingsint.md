---
title: "IRepTable2DColHeaderFooterIndiSettingsInt"
description: "The 2DTableColumnHeaderFooterIndividualSettings object provides the individual properties of table headers and footers in a 2D table in DIAdem REPORT."
---

# IRepTable2DColHeaderFooterIndiSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableColumnHeaderFooterIndividualSettings

The 2DTableColumnHeaderFooterIndividualSettings object provides the individual properties of table headers and footers in a 2D table in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyColumn1 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference = "[1]/[1]"
oMyColumn2 = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference = "[1]/[2]"
Col2HeadSettings = oMyColumn2.Settings.Header.IndividualSettings
Col2HeadSettings.Enable = True
Col2HeadSettings.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolheaderfooterindisettingsint-alignment/">Alignment</a> | <a href="../../properties/ireptable2dcolheaderfooterindisettingsint-angle/">Angle</a> | <a href="../../properties/ireptable2dcolheaderfooterindisettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/ireptable2dcolheaderfooterindisettingsint-enable/">Enable</a> | <a href="../../properties/ireptable2dcolheaderfooterindisettingsint-font/">Font</a> | <a href="../../properties/ireptable2dcolheaderfooterindisettingsint-usetextclipping/">UseTextClipping</a> | <a href="../../properties/ireptable2dcolheaderfooterindisettingsint-usewordwrap/">UseWordWrap</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dcolumnfootersettingsint/">2DTableColumnFooterSettings</a>.<a href="../../properties/ireptable2dcolumnfootersettingsint-individualsettings/">IndividualSettings</a> | <a href="../ireptable2dcolumnheadersettingsint/">2DTableColumnHeaderSettings</a>.<a href="../../properties/ireptable2dcolumnheadersettingsint-individualsettings/">IndividualSettings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColHeaderFooterIndiSettingsInt.htm`*
