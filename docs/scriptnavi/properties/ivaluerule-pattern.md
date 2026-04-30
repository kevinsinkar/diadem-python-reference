---
title: "IValueRule.Pattern"
description: "Specifies the search pattern of the Regular expression which DIAdem uses for a rule, when mapping values of a property. In addition to the Regular expressions o"
---

# IValueRule.Pattern

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Pattern for ValueRule

Specifies the search pattern of the Regular expression which DIAdem uses for a rule, when mapping values of a property. In addition to the Regular expressions of VBS, you can also use the ECMAScript syntax, for example ([[:alpha:]]+)([_\.;]+)([[:digit:]]+) .

## Signature

```python
obj.Pattern
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1~text~$3","Example_1")
print("Pattern: " , oMyRule.Pattern , "\r\n" , "Scheme: " , oMyRule.Schema , "\r\n" , "Example to map: " , oMyRule.Example , "\r\n" , "Mapped example: " , oMyRule.MapProperty(oMyRule.Example)) #Pattern => ([[:alpha:]],)([\_\-\/\\\?\ \:],)([[:digit:]],)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Pattern_IValueRule.htm`*
