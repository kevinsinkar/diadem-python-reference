---
title: "IDictionary.Item"
description: "Returns the Dictionary collection element that belongs to a specific key."
---

# IDictionary.Item

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Item for Dictionary

Returns the Dictionary collection element that belongs to a specific key.

## Signature

```python
obj.Item(Key)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
MyDic = CreateObject("Scripting.Dictionary")
MyDic.Add ("a", "Austin")
MyDic.Add ("b", "Berlin")
MyDic.Add ("c", "Chicago")
MyItem = MyDic.Item("b")
dd.MsgBox("Item b: " + MyItem)
```

```python
MyDic = CreateObject("Scripting.Dictionary")
MyArrA = Array("Austin", "Aachen", "Amsterdam")
MyArrB = Array("Berlin", "Bangalore", "Brussels")
MyArrC = Array("Chicago", "Cambridge", "Cannes")

MyDic.Add ("a", MyArrA)
MyDic.Add ("b", MyArrB)
MyDic.Add ("c", MyArrC)
MyItem = MyDic.Item("b")
sOutPut = "Elements of ""Item(b)"":" + VBCrLf
for MyArrayItem in MyItem:
    sOutPut = sOutPut + MyArrayItem + VBCrLf
dd.MsgBox(sOutPut)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Item_IDictionary.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
