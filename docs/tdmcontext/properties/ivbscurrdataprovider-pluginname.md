---
title: "IVbsCurrDataProvider.PluginName"
description: "Returns the name of the DataPlugin you use to open the data store."
---

# IVbsCurrDataProvider.PluginName

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: PluginName for CurrDataProvider <Analysis Automation>

Returns the name of the DataPlugin you use to open the data store.

## Signature

```python
obj.PluginName
```

## Python example

```python
def On_Initialize(oMyContext):
    oMyDataProvider = oContext.CurrDataProvider
    sMyPluginName = oContext.CurrDataProvider.PluginName
    if sMyPluginName == "" or len(sMyPluginName) == 0 :
#It is a DataFinder
        oMyDataFinder = dd.Navigator.ConnectDataFinderByParameter(oMyDataProvider.Parameters)
#...
    else:
#It is a DataStore
        oMyStore = dd.Navigator.ConnectDataStoreByParameter(oMyDataProvider.PluginName, oMyDataProvider.Parameters)
#...
        oMyStore.Close()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_PluginName_IVbsCurrDataProvider.htm`*
