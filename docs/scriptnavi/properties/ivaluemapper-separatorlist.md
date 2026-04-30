---
title: "IValueMapper.SeparatorList"
description: "Specifies an array with a separator which can be used when using a mapping rule, when mapping property values in the data preparation. This array is only for de"
---

# IValueMapper.SeparatorList

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: SeparatorList for PropertyValueMapper

Specifies an array with a separator which can be used when using a mapping rule, when mapping property values in the data preparation. This array is only for depositing the separator sign in the script API.

## Signature

```python
obj.SeparatorList
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyMapper.SeparatorList = ["_", "*", ":"]
MyList = oMyMapper.SeparatorList
print(MyList(0))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_SeparatorList_IValueMapper.htm`*
