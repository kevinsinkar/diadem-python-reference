---
title: "PropertyValueMappings"
description: "Collection of all PropertyValueMapping objects. Use the collection to access an individual object that combines the rules for a property in the data preparation"
---

# PropertyValueMappings

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: PropertyValueMappings

Collection of all PropertyValueMapping objects. Use the collection to access an individual object that combines the rules for a property in the data preparation.

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
<p><a href="../../properties/ivaluemappings-count/">Count</a> | <a href="../../properties/ivaluemappings-entityname/">EntityName</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivaluemappings-add/">Add</a> | <a href="../../methods/ivaluemappings-exists/">Exists</a> | <a href="../../methods/ivaluemappings-item/">Item</a> | <a href="../../methods/ivaluemappings-remove/">Remove</a> | <a href="../../methods/ivaluemappings-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../propertyentityvaluemappings/">PropertyEntityValueMappings</a>.<a href="../../methods/ientityvaluemappings-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IValueMappings.htm`*
