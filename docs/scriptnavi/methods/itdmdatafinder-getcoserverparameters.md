---
title: "ITDMDataFinder.GetCoServerParameters"
description: "Returns the parameters you use for opening the data currently open as a DataFinder instance, as an ASAM ODS data store. Use the ConnectDataStoreByParameter comm"
---

# ITDMDataFinder.GetCoServerParameters

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetCoServerParameters for DataFinder

Returns the parameters you use for opening the data currently open as a DataFinder instance, as an ASAM ODS data store. Use the ConnectDataStoreByParameter command to open the data with the parameters as an ASAM ODS data store (AOP5).

## Signature

```python
sGetCoServerParameters = Object.GetCoServerParameters()
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The <span class="Monospace">GetCoServerParameters</span> method only returns a value when a DataFinder instance was declared an ASAM ODS server.</td></tr></table>
</div>

## Python example

```python
oDataFinderServer = dd.Navigator.ConnectDataFinder("MyOwnDataFinder")
MyParams = oDataFinderServer.GetCoServerParameters()
dd.Navigator.ConnectDataStoreByParameter("NIAsamService",MyParams)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetCoServerParameters_ITDMDataFinder.htm`*
