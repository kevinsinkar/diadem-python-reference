---
title: "IRepTable2DColumnListInt.Move"
description: "Moves a table column in a 2D table in DIAdem REPORT to a different position."
---

# IRepTable2DColumnListInt.Move

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Move for 2DTableColumns

Moves a table column in a 2D table in DIAdem REPORT to a different position.

## Signature

```python
obj.Move(IndexFrom, MoveBeforeIndex)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMy2DColumns = oMy2DTable.Columns
oMyColumn1 = oMy2DColumns.Add(dd.e2DTableColumnChannel)
oMyColumn1.Channel.Reference= "[2]/[1]"
oMyColumn2 = oMy2DColumns.Add(dd.e2DTableColumnChannel)
oMyColumn2.Channel.Reference= "[2]/[2]"
oMyColumn3 = oMy2DColumns.Add(dd.e2DTableColumnChannel)
oMyColumn3.Channel.Reference= "[2]/[3]"
dd.Report.Refresh()
dd.Pause(5)
oMy2DColumns.Move(1,2)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Move_IRepTable2DColumnListInt.htm`*
