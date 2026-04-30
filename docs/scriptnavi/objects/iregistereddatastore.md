---
title: "IRegisteredDataStore"
description: "The RegisteredDataStore object provides the connection definition of a data store registered on your computer."
---

# IRegisteredDataStore

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: RegisteredDataStore <Navigator>

The RegisteredDataStore object provides the connection definition of a data store registered on your computer.

## Python example

```python
oMyDataStores = dd.Navigator.Settings.RegisteredDataStores
for Store in oMyDataStores:
    Output = Output + Store.Name + "\r\n"
dd.MsgBoxDisp("Registered DataStores: " + "\r\n" + output)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iregistereddatastore-datapluginname/">DataPluginName</a> | <a href="../../properties/iregistereddatastore-name/">Name</a> | <a href="../../properties/iregistereddatastore-parameter/">Parameter</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/registereddatastores/">RegisteredDataStores &lt;Navigator&gt;</a>.<a href="../../methods/iregistereddatastorecollection-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IRegisteredDataStore.htm`*
