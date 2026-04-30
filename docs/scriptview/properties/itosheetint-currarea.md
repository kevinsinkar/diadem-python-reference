---
title: "IToSheetInt.CurrArea"
description: "Returns the area in DIAdem VIEW that contains the formula expression which uses this property."
---

# IToSheetInt.CurrArea

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: CurrArea for Sheet

Returns the area in DIAdem VIEW that contains the formula expression which uses this property.

## Signature

```python
return_value = obj.CurrArea
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>You only can use this property in a user command, or in a script expression that you enclose in @@ characters.</td></tr></table>
</div>

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "TextBox"
oMyTextObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyTextObj.Text = "Name of this area: @@View.CurrSheet.CurrArea.Name@@"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_CurrArea_IToSheetInt.htm`*
