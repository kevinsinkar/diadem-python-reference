---
title: "ITDMDataStore.GetCoServerParameters"
description: "Returns the parameters for opening the data, which is currently open as an ASAM ODS data store, as a DataFinder instance. Use the ConnectDataFinderByParameter c"
---

# ITDMDataStore.GetCoServerParameters

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetCoServerParameters for DataStore

Returns the parameters for opening the data, which is currently open as an ASAM ODS data store, as a DataFinder instance. Use the ConnectDataFinderByParameter command to open the data as a DataFinder instance using parameters.

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
oMyDataStore = dd.Navigator.ConnectDataStore("ASAMTest1")
MyParams = oMyDataStore.GetCoServerParameters()
dd.Navigator.ConnectDataFinderByParameter(MyParams)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetCoServerParameters_ITDMDataStore.htm`*
