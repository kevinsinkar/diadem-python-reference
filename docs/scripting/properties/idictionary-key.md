---
title: "IDictionary.Key"
description: "Specifies the key for a Dictionary collection."
---

# IDictionary.Key

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Key for Dictionary

Specifies the key for a Dictionary collection.

## Signature

```python
obj.Key(Key)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
MyDic = win32com.client.Dispatch("Scripting.Dictionary")
MyDic.Add ("a", "Austin")
MyDic.Add ("b", "Berlin")
MyDic.Add ("c", "Chicago")
MyDic.Key("b") = "MyB"
MyItem = MyDic.Item("MyB")
dd.MsgBox("Item MyB: " + MyItem)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Key_IDictionary.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
