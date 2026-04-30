---
title: "ToBarInt.UsedActionObjs"
description: "Returns a collection of the elements of a bar."
---

# ToBarInt.UsedActionObjs

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: UsedActionObjs for Bar

Returns a collection of the elements of a bar.

## Signature

```python
return_value = obj.UsedActionObjs
```

## Python example

```python
objs = []
bar = dd.BarManager.Bars(1)
for obj in bar.UsedActionObjs:
    objs.append(obj.ID)
print("Bar:", bar.ID, objs)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_UsedActionObjs_ToBarInt.htm`*
