---
title: "IValueRules.Item"
description: "Returns a mapping rule associated with an index when mapping values of a property."
---

# IValueRules.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for ValueMappingRules

Returns a mapping rule associated with an index when mapping values of a property.

## Signature

```python
return_value = obj.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyPairs = oMyChnNameMapping.Rules
oMyPair1 = oMyChnNameMapping.Rules.AddPair("Example_1", "Example~1")
oMyPair2 = oMyChnNameMapping.Rules.AddPair("Example-2", "Example~2")
print("Pattern: " , oMyPairs.Item(1).Pattern) #Pattern => Example_1
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_IValueRules.htm`*
