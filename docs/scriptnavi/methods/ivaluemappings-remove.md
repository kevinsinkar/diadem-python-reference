---
title: "IValueMappings.Remove"
description: "Deletes the mapping with the specified name or index when mapping values of a property in the data preparation."
---

# IValueMappings.Remove

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Remove for PropertyValueMappings

Deletes the mapping with the specified name or index when mapping values of a property in the data preparation.

## Signature

```python
obj.Remove(NameOrIndex)
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1#$3","Example_1")
oMyMapper.Mappings(dd.eSearchChannel).Remove("name")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Remove_IValueMappings.htm`*
