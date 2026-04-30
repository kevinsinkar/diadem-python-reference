---
title: "IRegisteredDataStoreCollection.Exists"
description: "Checks whether the connection definition of a data store with the given name is registered on your computer."
---

# IRegisteredDataStoreCollection.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for RegisteredDataStores <Navigator>

Checks whether the connection definition of a data store with the given name is registered on your computer.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
oMyDataStores = dd.Navigator.Settings.RegisteredDataStores
dd.MsgBoxDisp(oMyDataStores.Exists("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_IRegisteredDataStoreCollection.htm`*
