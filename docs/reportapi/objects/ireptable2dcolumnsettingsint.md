---
title: "IRepTable2DColumnSettingsInt"
description: "The 2DTableColumnSettings object provides the properties of a 2D table header in DIAdem REPORT."
---

# IRepTable2DColumnSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableColumnSettings

The 2DTableColumnSettings object provides the properties of a 2D table header in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[2]"
oMyColumn.Settings.Alignment = dd.eTableAlignmentDecimalPoint
oMyColumn.Settings.Format = "d.dddd"
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumnsettingsint-alignment/">Alignment</a> | <a href="../../properties/ireptable2dcolumnsettingsint-angle/">Angle</a> | <a href="../../properties/ireptable2dcolumnsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/ireptable2dcolumnsettingsint-font/">Font</a> | <a href="../../properties/ireptable2dcolumnsettingsint-footer/">Footer</a> | <a href="../../properties/ireptable2dcolumnsettingsint-format/">Format</a> | <a href="../../properties/ireptable2dcolumnsettingsint-header/">Header</a> | <a href="../../properties/ireptable2dcolumnsettingsint-ondrawingcell/">OnDrawingCell</a> | <a href="../../properties/ireptable2dcolumnsettingsint-relativecolumnwidth/">RelativeColumnWidth</a> | <a href="../../properties/ireptable2dcolumnsettingsint-sortorder/">SortOrder</a> | <a href="../../properties/ireptable2dcolumnsettingsint-targetunit/">TargetUnit</a> | <a href="../../properties/ireptable2dcolumnsettingsint-usetextclipping/">UseTextClipping</a> | <a href="../../properties/ireptable2dcolumnsettingsint-usewordwrap/">UseWordWrap</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dcolumnbaseint/">2DTableColumn</a>.<a href="../../properties/ireptable2dcolumnbaseint-settings/">Settings</a> | <a href="../ireptable2dcolumnchannelint/">2DTableColumnChannel</a>.<a href="../../properties/ireptable2dcolumnchannelint-settings/">Settings</a> | <a href="../ireptable2dcolumnexpressionint/">2DTableColumnExpression</a>.<a href="../../properties/ireptable2dcolumnexpressionint-settings/">Settings</a> | <a href="../ireptable2dcolumntextint/">2DTableColumnText</a>.<a href="../../properties/ireptable2dcolumntextint-settings/">Settings</a> | <a href="../ireptable2dcolumnvariableint/">2DTableColumnVariable</a>.<a href="../../properties/ireptable2dcolumnvariableint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnSettingsInt.htm`*
