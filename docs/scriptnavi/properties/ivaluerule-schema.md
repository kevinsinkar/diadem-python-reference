---
title: "IValueRule.Schema"
description: "Specifies the replacement pattern according to which DIAdem replaces property values, when mapping the values of a property. The replacement patter may contain "
---

# IValueRule.Schema

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Schema for ValueRule

Specifies the replacement pattern according to which DIAdem replaces property values, when mapping the values of a property. The replacement patter may contain $ expressions and text. If the search pattern contains expressions in parentheses, you access the content of the parentheses with the $ expression in the replacement pattern. The regular expression saves the contents of the parenthesis according to their order in the expressions $1 , $2 , ... . For example, in the replacement pattern of the regular expression ([[:alpha:]]+)([_\.;]+)([[:digit:]]+) , the expression $1 contains the contents of the expression ([[:alpha:]]+) , $2 contains the contents of the expression ([_\.;]+) , and $3 contains the contents of the expression ([[:digit:]]+) . You can change the order of the $-expressions in the replacement pattern and additionally insert free text, for example "$1 AnyText $3$2” . Note Use Regular expressions to define search patterns. Besides the regular expressions of VBS, you can also use the ECMAScript syntax, for example ([[:alpha:]]+)([_\.;]+)([[:digit:]]+) .

## Signature

```python
obj.Schema
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use <a href="#" data-unresolved="1">Regular expressions</a> to define search patterns. Besides the regular expressions of VBS, you can also use the ECMAScript syntax, for example <span class="Monospace">([[:alpha:]]+)([_\.;]+)([[:digit:]]+)</span>.</td></tr></table>
</div>

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1~text~$3","Example_1")
print ("Pattern: " , oMyRule.Pattern , "\r\n" , "Schema: " , oMyRule.Schema , "\r\n" , "Example to map: " , oMyRule.Example , "\r\n" , "Mapped example: " , oMyRule.MapProperty(oMyRule.Example)) #Schema => $1~text~$3
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Schema_IValueRule.htm`*
