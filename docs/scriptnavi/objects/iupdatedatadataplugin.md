---
title: "IUpdateDataDataPlugin"
description: "You can use the UpdateDataDataPlugin object to access information about a DataPlugin in the update source."
---

# IUpdateDataDataPlugin

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: UpdateDataDataPlugin <Navigator>

You can use the UpdateDataDataPlugin object to access information about a DataPlugin in the update source.

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyUpdateData = oMyDataUpdateSource.UpdateData
dd.MsgBoxDisp(oMyUpdateData.Item(1).Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iupdatedatadataplugin-description/">Description</a> | <a href="../../properties/iupdatedatadataplugin-fileextensionlist/">FileExtensionList</a> | <a href="../../properties/iupdatedatadataplugin-name/">Name</a> | <a href="../../properties/iupdatedatadataplugin-type/">Type</a> | <a href="../../properties/iupdatedatadataplugin-url/">URL</a> | <a href="../../properties/iupdatedatadataplugin-version/">Version</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/updatedata/">UpdateData &lt;Navigator&gt;</a>.<a href="../../methods/iupdatedata-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IUpdateDataDataPlugin.htm`*
