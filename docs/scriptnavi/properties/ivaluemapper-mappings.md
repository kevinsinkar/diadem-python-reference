---
title: "IValueMapper.Mappings"
description: "Returns the collection of mappings of the file level (eSearchFile), channel group (eSearchChannelGroup), and channel (eSearchChannel), when mapping the values o"
---

# IValueMapper.Mappings

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Mappings for PropertyValueMapper

Returns the collection of mappings of the file level (eSearchFile), channel group (eSearchChannelGroup), and channel (eSearchChannel), when mapping the values of a property.

## Signature

```python
return_value = obj.Mappings
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

*Source: `ScriptNavi/properties/navigator_property_Mappings_IValueMapper.htm`*
