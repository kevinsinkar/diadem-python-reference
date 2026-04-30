---
title: "PropertyEntityValueMappings"
description: "Collection of the mappings of a specific level when mapping property values in the data preparation. A level can be a channel, a channel group, or a file."
---

# PropertyEntityValueMappings

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: PropertyEntityValueMappings

Collection of the mappings of a specific level when mapping property values in the data preparation. A level can be a channel, a channel group, or a file.

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1~text~$3","Example_1")
print("Pattern: " , oMyRule.Pattern , "\r\n" , "Scheme: " , oMyRule.Schema , "\r\n" , "Example to map: " , oMyRule.Example , "\r\n" , "Mapped example: " , oMyRule.MapProperty(oMyRule.Example))
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ientityvaluemappings-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ientityvaluemappings-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ivaluemapper/">PropertyValueMapper</a>.<a href="../../properties/ivaluemapper-mappings/">Mappings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IEntityValueMappings.htm`*
