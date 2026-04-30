---
title: "RegisteredDataStores"
description: "The RegisteredDataStores object provides the connection definitions of data stores registered on your computer."
---

# RegisteredDataStores

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: RegisteredDataStores <Navigator>

The RegisteredDataStores object provides the connection definitions of data stores registered on your computer.

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
<p><a href="../../properties/iregistereddatastorecollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iregistereddatastorecollection-exists/">Exists</a> | <a href="../../methods/iregistereddatastorecollection-item/">Item</a> | <a href="../../methods/iregistereddatastorecollection-remove/">Remove</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/inavigatorsettings/">Settings &lt;Navigator&gt;</a>.<a href="../../properties/inavigatorsettings-registereddatastores/">RegisteredDataStores</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IRegisteredDataStoreCollection.htm`*
