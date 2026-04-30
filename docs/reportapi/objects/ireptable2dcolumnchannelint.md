---
title: "IRepTable2DColumnChannelInt"
description: "The 2DTableColumnChannel object provides a 2D table column in DIAdem REPORT. The table column takes its contents from a channel."
---

# IRepTable2DColumnChannelInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableColumnChannel

The 2DTableColumnChannel object provides a 2D table column in DIAdem REPORT. The table column takes its contents from a channel.

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
oMyColumn.Settings.Font.Color.SetPredefinedColor(dd.ePredefinedColorRed)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumnchannelint-channel/">Channel</a> | <a href="../../properties/ireptable2dcolumnchannelint-index/">Index</a> | <a href="../../properties/ireptable2dcolumnchannelint-onchanneltransformation/">OnChannelTransformation</a> | <a href="../../properties/ireptable2dcolumnchannelint-settings/">Settings</a> | <a href="../../properties/ireptable2dcolumnchannelint-tagstored/">TagStored</a> | <a href="../../properties/ireptable2dcolumnchannelint-tagtemporary/">TagTemporary</a> | <a href="../../properties/ireptable2dcolumnchannelint-type/">Type</a> | <a href="../../properties/ireptable2dcolumnchannelint-useexpansion/">UseExpansion</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireptable2dcolumnchannelint-isexpanded/">IsExpanded</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-add/">Add</a> | <a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-changetype/">ChangeType</a> | <a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-copy/">Copy</a> | <a href="../../collections/2dtablecolumns/">2DTableColumns</a>.<a href="../../methods/ireptable2dcolumnlistint-item/">Item</a> | <a href="../ireptable2dcolumntransformingcontextint/">Table2DColumnTransformingContext</a>.<a href="../../properties/ireptable2dcolumntransformingcontextint-column/">Column</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnChannelInt.htm`*
