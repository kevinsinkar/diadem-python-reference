---
title: "ITDMStoreElements.Swap"
description: "Swaps the position of a data element with the position of another data element in a data store in DIAdem NAVIGATOR."
---

# ITDMStoreElements.Swap

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Swap for Elements <DataStore>

Swaps the position of a data element with the position of another data element in a data store in DIAdem NAVIGATOR.

## Signature

```python
obj.Swap(NameOrIndex1, NameOrIndex2)
```

## Python example

```python
dd.Navigator.ConnectDataStore("ASAM Browse Settings Example").RootElements(1).Children.Swap(1,2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Swap_ITDMStoreElements.htm`*
