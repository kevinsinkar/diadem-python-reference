---
title: "ValueMappingRules"
description: "Collection of properties and methods you use for defining the rules for mapping values of a property."
---

# ValueMappingRules

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: ValueMappingRules

Collection of properties and methods you use for defining the rules for mapping values of a property.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note </strong>Use the method <a href="../../methods/ivaluerules-addpair/">AddPair</a> to add a mapping rule for a 1:1 replacement.</td></tr></table>
</div>

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
<p><a href="../../properties/ivaluerules-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivaluerules-add/">Add</a> | <a href="../../methods/ivaluerules-addpair/">AddPair</a> | <a href="../../methods/ivaluerules-item/">Item</a> | <a href="../../methods/ivaluerules-remove/">Remove</a> | <a href="../../methods/ivaluerules-removeall/">RemoveAll</a> | <a href="../../methods/ivaluerules-swap/">Swap</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ivaluemapping/">PropertyValueMapping</a>.<a href="../../properties/ivaluemapping-rules/">Rules</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IValueRules.htm`*
