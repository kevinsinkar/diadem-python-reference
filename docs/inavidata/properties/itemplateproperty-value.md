---
title: "ITemplateProperty.Value"
description: "Specifies the initial value of a custom property from the custom properties template , in the script interface for internal data."
---

# ITemplateProperty.Value

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Value for TemplateProperty

Specifies the initial value of a custom property from the custom properties template , in the script interface for internal data.

## Signature

```python
obj.Value
```

## Python example

```python
oMyProp = dd.Data.Settings.CustomPropertyTemplate.ChannelProperties.Add("MyChnPropTemplate","",dd.DataTypeString)
oMyProp.Value = "test"
dd.Data.Root.ActiveChannelGroup.Channels.Add("MyChn",dd.DataTypeString)
dd.MsgBoxDisp (dd.Data.Root.ActiveChannelGroup.Channels("MyChn").Properties("MyChnPropTemplate").Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Value_ITemplateProperty.htm`*
