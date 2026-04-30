---
title: "IValueMappings.Exists"
description: "Checks whether a mapping already exists in the mapping collection for the specified property, when mapping values of a property in the data preparation."
---

# IValueMappings.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for PropertyValueMappings

Checks whether a mapping already exists in the mapping collection for the specified property, when mapping values of a property in the data preparation.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
if not oMyMapper.Mappings(dd.eSearchChannel).Exists("name") :
    oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
    oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1#$3","Example_1")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_IValueMappings.htm`*
