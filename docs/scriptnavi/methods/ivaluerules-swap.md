---
title: "IValueRules.Swap"
description: "Swaps the position of rules within the collection when mapping values of a property."
---

# IValueRules.Swap

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Swap for ValueMappingRules

Swaps the position of rules within the collection when mapping values of a property.

## Signature

```python
obj.Swap(IndexFrom, IndexTo)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note </strong> In rules with search pattern rules, all rules from 1 to n are executed. The mapping result corresponds with the first rule that can be applied without errors.</td></tr></table>
</div>

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRules = oMyChnNameMapping.Rules
oMyRule1 = oMyRules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1#$3","Example_1")
oMyRule2 = oMyRules.Add("([[:alpha:]]+)(#+)([[:digit:]]+)","$1$3","Example#1")
oMyRules.Swap(2,1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Swap_IValueRules.htm`*
