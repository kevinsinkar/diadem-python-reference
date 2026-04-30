---
title: "ITDMBrowseSettings.RootElements"
description: "Returns the elements that correspond to the root level of the browse path in a data store."
---

# ITDMBrowseSettings.RootElements

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: RootElements for BrowseSettings

Returns the elements that correspond to the root level of the browse path in a data store.

## Signature

```python
return_value = obj.RootElements
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEngineBrowseSettings = dd.Navigator.Settings.LoadBrowseSettings("D:\\MyEngineBrowseSettings.tbs", oMyDataStore)
#Active browse settings of data store
oMyRootElement = oMyDataStore.RootElements(1)
oMyChildren = oMyRootElement.Children
for Child in oMyChildren:
    dd.MsgBoxDisp("Data store" + "\r\n" + Child.Type + ": " + Child.Name)
#Browse settings of tbs file
oMyRootElement = oMyEngineBrowseSettings.RootElements(1)
oMyChildren = oMyEngineBrowseSettings.GetChildren(oMyRootElement)
for Child in oMyChildren:
    dd.MsgBoxDisp("Tbs file" + "\r\n" + Child.Type + ": " + Child.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_RootElements_ITDMBrowseSettings.htm`*
