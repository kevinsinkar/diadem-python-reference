---
title: "IValueMappings.Add"
description: "Adds a new mapping for a property, when mapping values of a property in the data preparation."
---

# IValueMappings.Add

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Add for PropertyValueMappings

Adds a new mapping for a property, when mapping values of a property in the data preparation.

## Signature

```python
return_value = obj.Add(PropertyName)
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1~text~$3","Example_1")
print("Pattern: " , oMyRule.Pattern , "\r\n" , "Scheme: " , oMyRule.Schema , "\r\n" , "Example to map: " , oMyRule.Example , "\r\n" , "Mapped example: " , oMyRule.MapProperty(oMyRule.Example))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Add_IValueMappings.htm`*
