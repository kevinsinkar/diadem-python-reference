---
title: "IRepTable2DColumnTextInt.TextList"
description: "Specifies the text list whose contents DIAdem REPORT displays in a 2D table column."
---

# IRepTable2DColumnTextInt.TextList

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TextList for 2DTableColumnText

Specifies the text list whose contents DIAdem REPORT displays in a 2D table column.

## Signature

```python
return_value = obj.TextList
```

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
oMyTextList = oMyColumn.TextList
oMyTextList.Count = 5
for I in range( 1, oMyTextList.Count+1):
    oMyTextList(I).Text = "Row " + I
oMy2DTable.Settings.IndexSettings.IndexMode = dd.e2DTableIndexModeAutomaticMinimum
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TextList_IRepTable2DColumnTextInt.htm`*
