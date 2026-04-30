---
title: "IValueMapping.PropertyName"
description: "Specifies the name of the property for which you created a mapping, when mapping values of a property."
---

# IValueMapping.PropertyName

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: PropertyName for PropertyValueMapping

Specifies the name of the property for which you created a mapping, when mapping values of a property.

## Signature

```python
obj.PropertyName
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1~text~$3","Example_1")
print("Property Name: " , oMyChnNameMapping.PropertyName , "\r\n" , "Pattern: " , oMyRule.Pattern , "\r\n" , "Scheme: " , oMyRule.Schema , "\r\n" , "Example to map: " , oMyRule.Example , "\r\n" , "Mapped example: " , oMyRule.MapProperty(oMyRule.Example))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_PropertyName_IValueMapping.htm`*
