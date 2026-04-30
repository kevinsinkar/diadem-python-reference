---
title: "IVbsContextAS.CurrDataProvider"
description: "Returns the CurrDataProvider <Analysis Automation> object which contains the properties of the current data store or DataFinder. Define the data source to use i"
---

# IVbsContextAS.CurrDataProvider

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: CurrDataProvider for ContextRun <Analysis Automation>

Returns the CurrDataProvider <Analysis Automation> object which contains the properties of the current data store or DataFinder. Define the data source to use in the associated task in the analysis automation. Use the CurrDataProvider <Analysis Automation> object to open a connection to the current DataFinder or data store with the ConnectDataFinderByParameter for Navigator and ConnectDataStoreByParameter for Navigator methods in order to execute additional searches there.

## Signature

```python
return_value = obj.CurrDataProvider
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
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

*Source: `TDMcontext/properties/TDMContext_property_CurrDataProvider_IVbsContextAS.htm`*
