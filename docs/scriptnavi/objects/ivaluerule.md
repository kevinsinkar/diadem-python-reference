---
title: "IValueRule"
description: "The ValueRule object provides a rule for mapping values of a property."
---

# IValueRule

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ValueRule

The ValueRule object provides a rule for mapping values of a property.

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyPair = oMyChnNameMapping.Rules.AddPair("Example_1", "Example~1")
dd.MsgBoxDisp ("Mapped Example: " + oMyPair.MapProperty("Example_1")) #Mapped Example => Example~1
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivaluerule-example/">Example</a> | <a href="../../properties/ivaluerule-pattern/">Pattern</a> | <a href="../../properties/ivaluerule-schema/">Schema</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivaluerule-getsubtoken/">GetSubToken</a> | <a href="../../methods/ivaluerule-mapproperty/">MapProperty</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/valuemappingrules/">ValueMappingRules</a>.<a href="../../methods/ivaluerules-add/">Add</a> | <a href="../../collections/valuemappingrules/">ValueMappingRules</a>.<a href="../../methods/ivaluerules-addpair/">AddPair</a> | <a href="../../collections/valuemappingrules/">ValueMappingRules</a>.<a href="../../methods/ivaluerules-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IValueRule.htm`*
