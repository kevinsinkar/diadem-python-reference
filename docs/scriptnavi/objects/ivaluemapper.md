---
title: "IValueMapper"
description: "The PropertyValueMapper object provides the mapping of property values in the data preparation."
---

# IValueMapper

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: PropertyValueMapper

The PropertyValueMapper object provides the mapping of property values in the data preparation.

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
<p><a href="../../properties/ivaluemapper-mappings/">Mappings</a> | <a href="../../properties/ivaluemapper-separatorlist/">SeparatorList</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavigatorsettings/">Settings &lt;Navigator&gt;</a>.<a href="../../methods/inavigatorsettings-createvaluemapper/">CreateValueMapper</a> | <a href="../inavigatorsettings/">Settings &lt;Navigator&gt;</a>.<a href="../../methods/inavigatorsettings-loadvaluemapper/">LoadValueMapper</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IValueMapper.htm`*
