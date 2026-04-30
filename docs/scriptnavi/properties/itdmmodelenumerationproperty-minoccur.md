---
title: "ITDMModelEnumerationProperty.MinOccur"
description: "Specifies in a data store the minimum number of values an enumeration property must contain. Note The MaxOccur property specifies the maximum number of values a"
---

# ITDMModelEnumerationProperty.MinOccur

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: MinOccur for ModelEnumerationProperty

Specifies in a data store the minimum number of values an enumeration property must contain. Note The MaxOccur property specifies the maximum number of values a property may contain. If MinOccur , for example, has the value 0 and MaxOccur has the value 1, the property may have a maximum value of 1 or no value. If MinOccur and MaxOccur have the value 1, the property must have exactly one value. If MinOccur has the value 1 and MaxOccur the value MaxInt , the property must have at least one value but can also have any number of values.

## Signature

```python
obj.MinOccur
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The <a href="../itdmmodelproperty-maxoccur/">MaxOccur</a> property specifies the maximum number of values a property may contain. If <span class="Monospace">MinOccur</span>, for example, has the value 0 and <span class="Monospace">MaxOccur</span> has the value 1, the property may have a maximum value of 1 or no value. If <span class="Monospace">MinOccur</span> and <span class="Monospace">MaxOccur</span> have the value 1, the property must have exactly one value. If <span class="Monospace">MinOccur</span> has the value 1 and <span class="Monospace">MaxOccur</span> the value <span class="Monospace">MaxInt</span>, the property must have at least one value but can also have any number of values.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyDataStoreModel = oMyDataStore.Model
dd.MsgBoxDisp(oMyDataStoreModel.Entities(1).ModelProperties(1).MinOccur)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_MinOccur_ITDMModelEnumerationProperty.htm`*
