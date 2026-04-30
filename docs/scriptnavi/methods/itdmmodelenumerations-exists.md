---
title: "ITDMModelEnumerations.Exists"
description: "Checks whether a specific enumeration property exists in the model of a data store."
---

# ITDMModelEnumerations.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for ModelEnumerations

Checks whether a specific enumeration property exists in the model of a data store.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEnums = oMyDataStore.Model.Enumerations
if oMyEnums.Exists("datatype") :
    for MyEnum in oMyEnums:
        sOutput = sOutput + "\r\n" + MyEnum.Name
    print("Enumerations of datatype: " + sOutput)
else:
    print("Enumeration not available")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_ITDMModelEnumerations.htm`*
