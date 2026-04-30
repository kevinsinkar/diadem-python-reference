---
title: "IValueMappings.EntityName"
description: "Returns the name of the associated level, when mapping the values of a property. A level can be a file (eSearchFile), a channel group (eSearchChannelGroup), or "
---

# IValueMappings.EntityName

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: EntityName for PropertyValueMappings

Returns the name of the associated level, when mapping the values of a property. A level can be a file (eSearchFile), a channel group (eSearchChannelGroup), or a channel (eSearchChannel).

## Signature

```python
obj.EntityName
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1~$3","Example_1")
print(oMyMapper.Mappings(dd.eSearchChannel).EntityName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_EntityName_IValueMappings.htm`*
