---
title: "IDataSettings.CustomPropertyTemplate"
description: "Specifies a custom properties template in the script interface for internal data."
---

# IDataSettings.CustomPropertyTemplate

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: CustomPropertyTemplate for Settings

Specifies a custom properties template in the script interface for internal data.

## Signature

```python
return_value = obj.CustomPropertyTemplate
```

## Python example

```python
oMyPropTemplate = dd.Data.Settings.CustomPropertyTemplate
oMyPropTemplate.ChannelProperties.Add("MyChnProp", 2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_CustomPropertyTemplate_IDataSettings.htm`*
