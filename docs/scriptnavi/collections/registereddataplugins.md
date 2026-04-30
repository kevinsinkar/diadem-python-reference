---
title: "RegisteredDataPlugins"
description: "Collection of all DataPlugins registered on your computer."
---

# RegisteredDataPlugins

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: RegisteredDataPlugins <Navigator>

Collection of all DataPlugins registered on your computer.

## Python example

```python
oMyDataPlugins = dd.Navigator.Settings.RegisteredDataPlugins
for DataPlugin in oMyDataPlugins:
    sOutput = sOutput + DataPlugin.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iregistereddataplugincollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iregistereddataplugincollection-exists/">Exists</a> | <a href="../../methods/iregistereddataplugincollection-item/">Item</a> | <a href="../../methods/iregistereddataplugincollection-remove/">Remove</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/inavigatorsettings/">Settings &lt;Navigator&gt;</a>.<a href="../../properties/inavigatorsettings-registereddataplugins/">RegisteredDataPlugins</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IRegisteredDataPluginCollection.htm`*
