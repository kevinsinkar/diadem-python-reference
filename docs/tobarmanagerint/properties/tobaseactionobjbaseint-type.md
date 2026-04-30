---
title: "ToBaseActionObjBaseInt.Type"
description: "Returns the bar element type."
---

# ToBaseActionObjBaseInt.Type

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Type for ActionObj

Returns the bar element type.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eActObjTypeButton` | 0 | The bar element is a button. |
| `eActObjTypeCheckButton` | 1 | The bar element is a button that displays a status. |
| `eActObjTypePopup` | 2 | The bar element is a button that opens a bar. |
| `eActObjTypeSeparator` | 3 | The bar element is a separator. |

## Python example

```python
dd.MsgBoxDisp("Type of second element: " + dd.BarManager.ActionObjs(2).Type)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Type_ToBaseActionObjBaseInt.htm`*
