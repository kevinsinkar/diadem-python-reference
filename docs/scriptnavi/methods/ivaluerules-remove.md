---
title: "IValueRules.Remove"
description: "Deletes the mapping rule with the specified index when mapping values of a property."
---

# IValueRules.Remove

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Remove for ValueMappingRules

Deletes the mapping rule with the specified index when mapping values of a property.

## Signature

```python
obj.Remove(Index)
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnDescriptionMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("description")
oMyRules = oMyChnDescriptionMapping.Rules
oMyRule1 = oMyRules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1$3","Example_1")
oMyRule2 = oMyRules.Add("([[:alpha:]])+(#)+([[:digit:]])+","$1$3","Example#1")
oMyRules.Remove(1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Remove_IValueRules.htm`*
