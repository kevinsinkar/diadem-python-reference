---
title: "UpdateData"
description: "List of the DataPlugins available in the update source."
---

# UpdateData

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: UpdateData <Navigator>

List of the DataPlugins available in the update source.

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyUpdateData = oMyDataUpdateSource.UpdateData
dd.MsgBoxDisp(oMyUpdateData.Item(1).Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iupdatedata-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iupdatedata-exists/">Exists</a> | <a href="../../methods/iupdatedata-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/iupdatesource/">UpdateSource &lt;Navigator&gt;</a>.<a href="../../properties/iupdatesource-updatedata/">UpdateData</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IUpdateData.htm`*
