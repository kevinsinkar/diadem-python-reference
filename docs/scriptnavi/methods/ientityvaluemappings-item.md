---
title: "IEntityValueMappings.Item"
description: "Returns the level on which the mapping for a property is defined, when mapping property values in the data preparation."
---

# IEntityValueMappings.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for PropertyEntityValueMappings

Returns the level on which the mapping for a property is defined, when mapping property values in the data preparation.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSearchRoot` | 1 | Mapping in root properties |
| `eSearchChannelGroup` | 2 | Mapping in group properties |
| `eSearchChannel` | 3 | Mapping in channel properties |

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyMapping = oMyMapper.Mappings
print(oMyMapping.Item(dd.eSearchChannel).EntityName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_IEntityValueMappings.htm`*
