---
title: "ITDMModelEnumerations.Count"
description: "Specifies the number of enumerations in the model of a data store."
---

# ITDMModelEnumerations.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for ModelEnumerations

Specifies the number of enumerations in the model of a data store.

## Signature

```python
obj.Count
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEnums = oMyDataStore.Model.Enumerations
print(oMyEnums.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_ITDMModelEnumerations.htm`*
