---
title: "ITDMModelEnumerationProperty.MaxOccur"
description: "Specifies in a data store the maximum number of values an enumeration property may contain. Note The MinOccur property specifies the minimum number of values a "
---

# ITDMModelEnumerationProperty.MaxOccur

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: MaxOccur for ModelEnumerationProperty

Specifies in a data store the maximum number of values an enumeration property may contain. Note The MinOccur property specifies the minimum number of values a property must contain. If MinOccur , for example, has the value 0 and MaxOccur has the value 1, the property may have a maximum value of 1 or no value. If MinOccur and MaxOccur have the value 1, the property must have exactly one value. If MinOccur has the value 1 and MaxOccur the value MaxInt , the property must have at least one value but can also have any number of values.

## Signature

```python
obj.MaxOccur
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The <a href="../itdmmodelproperty-minoccur/">MinOccur</a> property specifies the minimum number of values a property must contain. If <span class="Monospace">MinOccur</span>, for example, has the value 0 and <span class="Monospace">MaxOccur</span> has the value 1, the property may have a maximum value of 1 or no value. If <span class="Monospace">MinOccur</span> and <span class="Monospace">MaxOccur</span> have the value 1, the property must have exactly one value. If <span class="Monospace">MinOccur</span> has the value 1 and <span class="Monospace">MaxOccur</span> the value <span class="Monospace">MaxInt</span>, the property must have at least one value but can also have any number of values.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyDataStoreModel = oMyDataStore.Model
dd.MsgBoxDisp(oMyDataStoreModel.Entities(1).ModelProperties(1).MaxOccur)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_MaxOccur_ITDMModelEnumerationProperty.htm`*
