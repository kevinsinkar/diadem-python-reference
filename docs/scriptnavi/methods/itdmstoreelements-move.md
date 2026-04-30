---
title: "ITDMStoreElements.Move"
description: "Moves a data element to a different position in a data store in DIAdem NAVIGATOR."
---

# ITDMStoreElements.Move

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Move for Elements <DataStore>

Moves a data element to a different position in a data store in DIAdem NAVIGATOR.

## Signature

```python
obj.Move(NameOrIndex, Position)
```

## Python example

```python
dd.Navigator.ConnectDataStore("ASAM Browse Settings Example").RootElements(1).Children.Move(1,2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Move_ITDMStoreElements.htm`*
