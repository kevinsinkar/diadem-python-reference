---
title: "IRepCtrlListInt.Item"
description: "Returns the object that is associated with a specific name or with a specific index."
---

# IRepCtrlListInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for ReportObjects

Returns the object that is associated with a specific name or with a specific index.

## Signature

```python
return_value = obj.Item(NameOrIndex)
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
sOutput = ""
oMyObjects = dd.Report.ActiveSheet.Objects
for i in range( 1, oMyObjects.Count+1):
    sOutput = sOutput + "Object type: " + oMyObjects.Item(i).ObjectType + "\t" + "Element name: " + oMyObjects.Item(i).Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepCtrlListInt.htm`*
