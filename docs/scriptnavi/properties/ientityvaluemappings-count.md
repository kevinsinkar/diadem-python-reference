---
title: "IEntityValueMappings.Count"
description: "Returns the number of possible levels on which you can define the mappings for properties, when mapping the values of a property in the data preparation. A leve"
---

# IEntityValueMappings.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for PropertyEntityValueMappings

Returns the number of possible levels on which you can define the mappings for properties, when mapping the values of a property in the data preparation. A level can be a file (eSearchFile), a channel group (eSearchChannelGroup), or a channel (eSearchChannel). The number of levels is always 3.

## Signature

```python
obj.Count
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyMappings = oMyMapper.Mappings
print(oMyMappings.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_IEntityValueMappings.htm`*
