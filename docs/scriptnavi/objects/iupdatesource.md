---
title: "IUpdateSource"
description: "Use the UpdateSource object to access general information about DataPlugins on the NI DataPlugin website or on a DataFinder instance."
---

# IUpdateSource

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: UpdateSource <Navigator>

Use the UpdateSource object to access general information about DataPlugins on the NI DataPlugin website or on a DataFinder instance.

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
dd.MsgBoxDisp("Last update: " + oMyDataUpdateSource.LastUpdate + "\r\n" + "Number of DataPlugins: " + oMyDataUpdateSource.UpdateData.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iupdatesource-lastupdate/">LastUpdate</a> | <a href="../../properties/iupdatesource-parameter/">Parameter</a> | <a href="../../properties/iupdatesource-type/">Type</a> | <a href="../../properties/iupdatesource-updatedata/">UpdateData</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iupdatesource-compareversion/">CompareVersion</a> | <a href="../../methods/iupdatesource-find/">Find</a> | <a href="../../methods/iupdatesource-install/">Install</a> | <a href="../../methods/iupdatesource-update/">Update</a> | <a href="../../methods/iupdatesource-updateall/">UpdateAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavigatorsettings/">Settings &lt;Navigator&gt;</a>.<a href="../../methods/inavigatorsettings-createupdatesource/">CreateUpdateSource</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IUpdateSource.htm`*
