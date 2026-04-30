---
title: "IRepExpansionLineStyleListInt.Item"
description: "Returns the settings of a specific index, which DIAdem uses for curve displays with Curve expansion in DIAdem REPORT layouts."
---

# IRepExpansionLineStyleListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for ExpansionLineStyles

Returns the settings of a specific index, which DIAdem uses for curve displays with Curve expansion in DIAdem REPORT layouts.

## Signature

```python
return_value = obj.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
oMyCurveExpandObj = dd.Report.Settings.CurveExpansion
oMyExpandLine = oMyCurveExpandObj.AttributeList.LineStyles
oMyCurveExpandObj.Enable = True
oMyCurveExpandObj.AttributeList.Enable = True
for I in range( 1, oMyExpandLine.Count+1):
    oMyExpandLine.Item(I).Line.Width = dd.eLineWidth0070
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepExpansionLineStyleListInt.htm`*
