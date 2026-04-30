---
title: "IValueRules.Count"
description: "Returns the number of rules defined for this property, when mapping the values of a property."
---

# IValueRules.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for ValueMappingRules

Returns the number of rules defined for this property, when mapping the values of a property.

## Signature

```python
obj.Count
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyPairs = oMyChnNameMapping.Rules
oMyPair1 = oMyChnNameMapping.Rules.AddPair("Example_1", "Example~1")
oMyPair2 = oMyChnNameMapping.Rules.AddPair("Example-2", "Example~2")
print ("Number of rules: " , oMyPairs.Count) #Number of rules: 2
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_IValueRules.htm`*
