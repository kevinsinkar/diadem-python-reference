---
title: "IRepTable2DColumnVariableInt"
description: "The 2DTableColumnVariable object provides a 2D table column in DIAdem REPORT. The table column takes its contents from a variable."
---

# IRepTable2DColumnVariableInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableColumnVariable

The 2DTableColumnVariable object provides a 2D table column in DIAdem REPORT. The table column takes its contents from a variable.

## Python example

```python
dd.Report.NewLayout()
oMy2DTable = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DTable,"My2DTable")
oMyPosition = oMy2DTable.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnVariable)
oMyColumn.VariableName = "CurrTime"
oMyColumn.Settings.Font.Color.SetPredefinedColor(dd.ePredefinedColorBlue)
oMy2DTable.Settings.IndexSettings.IndexMode = dd.e2DTableIndexModeAutomaticMinimum
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2dcolumnvariableint-index/">Index</a> | <a href="../../properties/ireptable2dcolumnvariableint-settings/">Settings</a> | <a href="../../properties/ireptable2dcolumnvariableint-tagstored/">TagStored</a> | <a href="../../properties/ireptable2dcolumnvariableint-tagtemporary/">TagTemporary</a> | <a href="../../properties/ireptable2dcolumnvariableint-type/">Type</a> | <a href="../../properties/ireptable2dcolumnvariableint-variablename/">VariableName</a></p>
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

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DColumnVariableInt.htm`*
