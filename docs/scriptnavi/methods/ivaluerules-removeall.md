---
title: "IValueRules.RemoveAll"
description: "Deletes all property mapping rules when mapping the values of a property."
---

# IValueRules.RemoveAll

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: RemoveAll for ValueMappingRules

Deletes all property mapping rules when mapping the values of a property.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRules = oMyChnNameMapping.Rules
oMyRule1 = oMyRules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1#$3","Example_1")
oMyRule2 = oMyRules.Add("([[:alpha:]]+)(#+)([[:digit:]]+)","$1$3","Example#1")
print("Number of rules before deleting: " + oMyRules.Count) #Number of rules before deleting: 2
oMyRules.RemoveAll()
print("Number of rules after deleting: " + oMyRules.Count) #Number of rules after deleting: 0
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_RemoveAll_IValueRules.htm`*
