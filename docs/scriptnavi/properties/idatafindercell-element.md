---
title: "IDataFinderCell.Element"
description: "Returns the element which is associated to a cell, in the search results list of a DataFinder."
---

# IDataFinderCell.Element

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Element for Cell <DataFinder>

Returns the element which is associated to a cell, in the search results list of a DataFinder.

## Signature

```python
return_value = obj.Element
```

## Python example

```python
oMyResultsList = dd.Navigator.Display.CurrDataFinder.ResultsList
oMyCell = oMyResultsList.FocusedCell
dd.MsgBoxDisp(oMyCell.Element.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Element_IDataFinderCell.htm`*
