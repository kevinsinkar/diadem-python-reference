---
title: "IValueMappings.Item"
description: "Returns the mapping object associated with a specific name or index, when mapping values of a property in the data preparation."
---

# IValueMappings.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for PropertyValueMappings

Returns the mapping object associated with a specific name or index, when mapping values of a property in the data preparation.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1#$3","Example_1")
print(oMyMapper.Mappings(dd.eSearchChannel).Item("name").PropertyName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_IValueMappings.htm`*
