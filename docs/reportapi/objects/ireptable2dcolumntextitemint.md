---
title: "IRepTable2DColumnTextItemInt"
description: "The 2DTableColumnTextItem object provides a text from a text list from which a 2D table column in DIAdem REPORT takes the contents."
---

# IRepTable2DColumnTextItemInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableColumnTextItem

The 2DTableColumnTextItem object provides a text from a text list from which a 2D table column in DIAdem REPORT takes the contents.

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnText)
oMyColumn.Settings.Font.Color.SetPredefinedColor(dd.ePredefinedColorBlue)
oMyTextList = oMyColumn.TextList
oMyTextList.Count = 5
for I in range( 1, oMyTextList.Count+1):
    oMyTextList(I).Text = "Row " + I

oMy2DTable.Settings.IndexSettings.IndexMode = dd.e2DTableIndexModeAutomaticMinimum
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumntextitemint-text/">Text</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/2dtablecolumntextlist/">2DTableColumnTextList</a>.<a href="../../methods/ireptable2dcolumntextlistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnTextItemInt.htm`*
