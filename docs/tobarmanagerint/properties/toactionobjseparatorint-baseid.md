---
title: "ToActionObjSeparatorInt.BaseID"
description: "Specifies the name of the base type of a bar element. There are base types for user-defined bar elements and predefined base types for a specific purpose. User-"
---

# ToActionObjSeparatorInt.BaseID

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: BaseID for ActionObjSeparator

Specifies the name of the base type of a bar element. There are base types for user-defined bar elements and predefined base types for a specific purpose. User-defined base types always start with the ID Custom , such as CustomButton and CustomPopup .

## Signature

```python
obj.BaseID
```

## Python example

```python
def MyReset(oMyObject):
    if oMyObject.BaseId != "Separator" :
        oMyObject.ResetTooltip()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_BaseID_ToActionObjSeparatorInt.htm`*
