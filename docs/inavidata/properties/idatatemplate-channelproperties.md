---
title: "IDataTemplate.ChannelProperties"
description: "Specifies the custom properties of channels in the custom properties template , in the script interface for internal data."
---

# IDataTemplate.ChannelProperties

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: ChannelProperties for CustomPropertyTemplate

Specifies the custom properties of channels in the custom properties template , in the script interface for internal data.

## Signature

```python
return_value = obj.ChannelProperties
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the methods and properties from the <a href="../../collections/properties/">Properties</a> collection to work within a <a href="#" data-unresolved="1">Template</a> with custom properties of channels. These methods and properties are in the script interface Help for internal data.</td></tr></table>
</div>

## Python example

```python
oMyPropTemplate= dd.Data.Settings.CustomPropertyTemplate
oMyPropTemplate.ChannelProperties.Add("MyChnProp", 2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_ChannelProperties_IDataTemplate.htm`*
