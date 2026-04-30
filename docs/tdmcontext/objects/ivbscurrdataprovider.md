---
title: "IVbsCurrDataProvider"
description: "The CurrDataProvider <Analysis Automation> object provides the properties of the current data store or DataFinder. Define the data source to use in the associat"
---

# IVbsCurrDataProvider

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: CurrDataProvider <Analysis Automation>

The CurrDataProvider <Analysis Automation> object provides the properties of the current data store or DataFinder. Define the data source to use in the associated task in the analysis automation. Use the CurrDataProvider <Analysis Automation> object to open a connection to the current DataFinder or data store with the ConnectDataFinderByParameter for Navigator and ConnectDataStoreByParameter for Navigator methods in order to execute additional searches there.

## Python example

```python
def On_Initialize(oContext):
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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbscurrdataprovider-parameters/">Parameters</a> | <a href="../../properties/ivbscurrdataprovider-pluginname/">PluginName</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ivbscontextasdeinit/">ContextFinalize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasdeinit-currdataprovider/">CurrDataProvider</a> | <a href="../ivbscontextasinit/">ContextInitialize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasinit-currdataprovider/">CurrDataProvider</a> | <a href="../ivbscontextas/">ContextRun &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextas-currdataprovider/">CurrDataProvider</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsCurrDataProvider.htm`*
