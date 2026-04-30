---
title: "IRepTable2DColumnExpressionInt.Type"
description: "Specifies whether the column of a 2D table in DIAdem REPORT contains data channels, variables, DIAdem expressions, or text lists."
---

# IRepTable2DColumnExpressionInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 2DTableColumnExpression

Specifies whether the column of a 2D table in DIAdem REPORT contains data channels, variables, DIAdem expressions, or text lists.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `Expression` | 2 | e2DTableColumnExpression |

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        for oMyColumn in oMyReportObj.Columns:
            sOutput = sOutput + "Object name: " + oMyReportObj.Name + "\t" + "Column typ: " +  oMyColumn.Type + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepTable2DColumnExpressionInt.htm`*
