---
title: "ITDMStoreReference.BaseName"
description: "Specifies in a data storage the base name of the reference of an Element object."
---

# ITDMStoreReference.BaseName

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: BaseName for Reference

Specifies in a data storage the base name of the reference of an Element object.

## Signature

```python
obj.BaseName
```

## Python example

```python
oMyDataStore = dd.NAVIGATOR.ConnectDataStore("ASAM Browse Settings Example")
oMyRootElement = oMyDataStore.RootElements(1)
oMyTest = oMyRootElement.Children(1)
oMyMeasurement = oMyTest.Children(1)
for Reference in oMyMeasurement.References:
    dd.MsgBoxDisp("BaseName: " + Reference.BaseName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_BaseName_ITDMStoreReference.htm`*
