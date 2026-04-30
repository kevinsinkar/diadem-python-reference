---
title: "ITDMStoreElement.DisplayName"
description: "Specifies in a data store the display name of an element."
---

# ITDMStoreElement.DisplayName

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: DisplayName for Element <DataStore>

Specifies in a data store the display name of an element.

## Signature

```python
obj.DisplayName
```

## Python example

```python
oMyDataStore = dd.NAVIGATOR.ConnectDataStore("ASAM Browse Settings Example")
oMyRootElement = oMyDataStore.RootElements(1)
oMyElements = oMyRootElement.Children
for Element in oMyElements:
    dd.MsgBoxDisp(Element.DisplayName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_DisplayName_ITDMStoreElement.htm`*
