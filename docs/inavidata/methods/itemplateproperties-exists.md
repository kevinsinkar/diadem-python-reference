---
title: "ITemplateProperties.Exists"
description: "Checks whether a TemplateProperty object with a specific name already exists in the collection of custom properties templates in the script interface for intern"
---

# ITemplateProperties.Exists

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Exists for TemplateProperties

Checks whether a TemplateProperty object with a specific name already exists in the collection of custom properties templates in the script interface for internal data.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
oMyPropTemplate = dd.Data.Settings.CustomPropertyTemplate
dd.MsgBoxDisp(oMyPropTemplate.RootProperties.Exists("MyRootProp"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Exists_ITemplateProperties.htm`*
