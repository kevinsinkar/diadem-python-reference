---
title: "Dictionary"
description: "The Dictionary object provides an array with a key/element pair. The key and the element can have any data type, but the key cannot be an array. A Dictionary ob"
---

# Dictionary

!!! abstract "Collection &middot; `Scripting.chm`"
    Collection: Dictionary

The Dictionary object provides an array with a key/element pair. The key and the element can have any data type, but the key cannot be an array. A Dictionary object is comparable with an associative array. To use the Dictionary object, you must create this object in DIAdem with the CreateObject("Scripting.Dictionary") command.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
MyDic = CreateObject("Scripting.Dictionary")
MyDic.Add("a", "Austin")
MyDic.Add("b", "Berlin")
MyDic.Add("c", "Chicago")
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
sOutPut = "Elements of ""Item(b)"":" + "\r\n"
for MyArrayItem in MyItem:
    sOutPut = sOutPut + MyArrayItem + "\r\n"
dd.MsgBox(sOutPut)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idictionary-comparemode/">CompareMode</a> | <a href="../../properties/idictionary-count/">Count</a> | <a href="../../properties/idictionary-item/">Item</a> | <a href="../../properties/idictionary-key/">Key</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idictionary-add/">Add</a> | <a href="../../methods/idictionary-exists/">Exists</a> | <a href="../../methods/idictionary-items/">Items</a> | <a href="../../methods/idictionary-keys/">Keys</a> | <a href="../../methods/idictionary-remove/">Remove</a> | <a href="../../methods/idictionary-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/objects/Scripting_Objects_IDictionary.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
