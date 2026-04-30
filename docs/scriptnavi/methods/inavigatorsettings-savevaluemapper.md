---
title: "INavigatorSettings.SaveValueMapper"
description: "Saves a file for the mapping of values of a property, in the data preparation. In a mapping you use rules to replace property values. Mapping files have the fil"
---

# INavigatorSettings.SaveValueMapper

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: SaveValueMapper for Settings <Navigator>

Saves a file for the mapping of values of a property, in the data preparation. In a mapping you use rules to replace property values. Mapping files have the filename extension *.TPVM (Technical Property Value Mapping).

## Signature

```python
obj.SaveValueMapper(FileName, pValueMapper)
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([A-Za-z]+)([\\_\\-\\/\\\\?\\ \\:]+)([0-9]+)","$1$3","Example_1")
dd.Navigator.Settings.SaveValueMapper("D:\\MyValueMapper.tpmv", oMyMapper)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_SaveValueMapper_INavigatorSettings.htm`*
