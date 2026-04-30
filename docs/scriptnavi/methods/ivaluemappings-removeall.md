---
title: "IValueMappings.RemoveAll"
description: "Deletes all property mappings on the specified level when mapping the values of a property in the data preparation."
---

# IValueMappings.RemoveAll

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: RemoveAll for PropertyValueMappings

Deletes all property mappings on the specified level when mapping the values of a property in the data preparation.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1#$3","Example_1")
oMyMapper.Mappings(dd.eSearchChannel).RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_RemoveAll_IValueMappings.htm`*
