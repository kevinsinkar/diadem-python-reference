---
title: "IValueMappings.Count"
description: "Returns the number of mappings defined for a level, when mapping the values of a property. A level can be a file (eSearchFile), a channel group (eSearchChannelG"
---

# IValueMappings.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for PropertyValueMappings

Returns the number of mappings defined for a level, when mapping the values of a property. A level can be a file (eSearchFile), a channel group (eSearchChannelGroup), or a channel (eSearchChannel).

## Signature

```python
obj.Count
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[digit:]]+)","$1~$3","Example_1")
print(oMyMapper.Mappings(dd.eSearchChannel).Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_IValueMappings.htm`*
