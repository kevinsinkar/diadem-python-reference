---
title: "IDictionary.Items"
description: "Returns an array with the elements from a Dictionary collection."
---

# IDictionary.Items

!!! abstract "Method &middot; `Scripting.chm`"
    Method: Items for Dictionary

Returns an array with the elements from a Dictionary collection.

## Signature

```python
vItems = Object.Items
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
MyDic = CreateObject("Scripting.Dictionary")
MyDic.Add("a", "Austin")
MyDic.Add("b", "Berlin")
MyDic.Add("c", "Chicago")
MyItems = MyDic.Items
for MyItem in MyItems:
    sOutput = sOutput + MyItem + VBCrLf
dd.MsgBox(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_Items_IDictionary.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
