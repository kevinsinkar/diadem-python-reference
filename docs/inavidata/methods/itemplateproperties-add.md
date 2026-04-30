---
title: "ITemplateProperties.Add"
description: "Generates a new custom properties template with a value in the script interface for internal data. If the custom properties template already exists, DIAdem chan"
---

# ITemplateProperties.Add

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Add for TemplateProperties

Generates a new custom properties template with a value in the script interface for internal data. If the custom properties template already exists, DIAdem changes only the value of this custom properties template. If the custom properties template does not exist, DIAdem creates a new custom properties template. The Add method returns a TemplateProperty object.

## Signature

```python
return_value = obj.Add(Name, Value, [DataType])
```

## Notes

<div markdown="1">
<table class="Borderless" id="table3"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The value of the custom property must correspond to the specified data type.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `Enumeration` | 24 | DataTypeEnum |

## Python example

```python
oMyPropTemplate = dd.Data.Settings.CustomPropertyTemplate
oMyPropTemplate.RootProperties.Add("MyRootProp", 2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Add_ITemplateProperties.htm`*
