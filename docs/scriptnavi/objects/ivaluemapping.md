---
title: "IValueMapping"
description: "The PropertyValueMapping mapping combines all rule for mapping a property in the data preparation."
---

# IValueMapping

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: PropertyValueMapping

The PropertyValueMapping mapping combines all rule for mapping a property in the data preparation.

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
<p><a href="../../properties/ivaluemapping-propertyname/">PropertyName</a> | <a href="../../properties/ivaluemapping-rules/">Rules</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivaluemapping-mapproperty/">MapProperty</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/propertyvaluemappings/">PropertyValueMappings</a>.<a href="../../methods/ivaluemappings-add/">Add</a> | <a href="../../collections/propertyvaluemappings/">PropertyValueMappings</a>.<a href="../../methods/ivaluemappings-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IValueMapping.htm`*
