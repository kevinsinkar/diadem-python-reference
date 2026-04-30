---
title: "IValueRule.Example"
description: "Specifies an example text with which DIAdem can check a defined rule when mapping values of a property."
---

# IValueRule.Example

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Example for ValueRule

Specifies an example text with which DIAdem can check a defined rule when mapping values of a property.

## Signature

```python
obj.Example
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1~text~$3","Example_1")
print ("Pattern: " , oMyRule.Pattern , "\r\n" , "Scheme: " , oMyRule.Schema , "\r\n" , "Example to map: " , oMyRule.Example , "\r\n" , "Mapped example: " , oMyRule.MapProperty(oMyRule.Example)) #Mapped example =>  Example~text~1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Example_IValueRule.htm`*
