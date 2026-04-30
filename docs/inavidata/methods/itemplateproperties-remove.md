---
title: "ITemplateProperties.Remove"
description: "Deletes a custom property from the TemplateProperties collection in the script interface for internal data."
---

# ITemplateProperties.Remove

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Remove for TemplateProperties

Deletes a custom property from the TemplateProperties collection in the script interface for internal data.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyPropTemplate = dd.Data.Settings.CustomPropertyTemplate
oMyPropTemplate.RootProperties.Remove("MyRootProp")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Remove_ITemplateProperties.htm`*
