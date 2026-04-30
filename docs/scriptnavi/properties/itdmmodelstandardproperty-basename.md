---
title: "ITDMModelStandardProperty.BaseName"
description: "Specifies in the data model of a data store the base name of a standard property."
---

# ITDMModelStandardProperty.BaseName

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: BaseName for ModelStandardProperty

Specifies in the data model of a data store the base name of a standard property.

## Signature

```python
obj.BaseName
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyDataStoreModel = oMyDataStore.Model
dd.MsgBoxDisp(oMyDataStoreModel.Entities("MeaQuantity").ModelProperties(1).BaseName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_BaseName_ITDMModelStandardProperty.htm`*
