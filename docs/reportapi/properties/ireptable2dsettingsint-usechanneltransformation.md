---
title: "IRepTable2DSettingsInt.UseChannelTransformation"
description: "Specifies whether DIAdem REPORT enables the Channel Transformation in a 2D table."
---

# IRepTable2DSettingsInt.UseChannelTransformation

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseChannelTransformation for 2DTableSettings

Specifies whether DIAdem REPORT enables the Channel Transformation in a 2D table.

## Signature

```python
obj.UseChannelTransformation
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
oMyColumn = oMy2DTable.Columns.Add(dd.e2DTableColumnChannel)
oMyColumn.Channel.Reference = "[1]/[2]"
oMyColumn.Settings.Alignment = dd.eTableAlignmentDecimalPoint
oMyColumn.Settings.Format = "d.dddd"
oMy2DTable.Settings.UseChannelTransformation = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseChannelTransformation_IRepTable2DSettingsInt.htm`*
