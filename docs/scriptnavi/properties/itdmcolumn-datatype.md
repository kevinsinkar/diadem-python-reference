---
title: "ITDMColumn.DataType"
description: "Specifies the data type of a properties column in the search results. Note DIAdem automatically specifies the data type of base properties and optimized custom "
---

# ITDMColumn.DataType

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: DataType for Column

Specifies the data type of a properties column in the search results. Note DIAdem automatically specifies the data type of base properties and optimized custom properties. Use the Add method to specify the data type of non-optimized custom properties.

## Signature

```python
obj.DataType
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  DIAdem automatically specifies the data type of base properties and optimized custom properties. Use the <a href="../../methods/itdmcolumns-add/">Add</a> method to specify the data type of non-optimized custom properties.</td></tr></table>
</div>

## Python example

```python
oMyResultsList = dd.Navigator.Display.CurrDataFinder.ResultsList
dd.MsgBoxDisp(oMyResultsList.Columns(1).DataType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_DataType_ITDMColumn.htm`*
