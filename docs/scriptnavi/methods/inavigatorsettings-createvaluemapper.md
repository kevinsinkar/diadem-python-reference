---
title: "INavigatorSettings.CreateValueMapper"
description: "Creates a ValueMapping object for the data preparation. In a ValueMapping you use rules to replace property values."
---

# INavigatorSettings.CreateValueMapper

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: CreateValueMapper for Settings <Navigator>

Creates a ValueMapping object for the data preparation. In a ValueMapping you use rules to replace property values.

## Signature

```python
return_value = obj.CreateValueMapper()
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([A-Za-z]+)([\\_\\-\\/\\\\?\\ \\:]+)([0-9]+)","$1#$3","Example_1")
print("Pattern: " , oMyRule.Pattern , "\r\n" , "Scheme: " , oMyRule.Schema , "\r\n" , "Example: " , oMyRule.Example , "\r\n" , "Mapping: " , oMyRule.MapProperty(oMyRule.Example), "\r\n" , "Mapping: " , oMyRule.MapProperty("Pascalstreet_18"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_CreateValueMapper_INavigatorSettings.htm`*
