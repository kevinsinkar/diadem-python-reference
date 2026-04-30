---
title: "IDictionary.Exists"
description: "Checks whether there is a key in a Dictionary collection."
---

# IDictionary.Exists

!!! abstract "Method &middot; `Scripting.chm`"
    Method: Exists for Dictionary

Checks whether there is a key in a Dictionary collection.

## Signature

```python
bExists = Object.Exists(Key)
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
if MyDic.Exists("a"):
    dd.MsgBox("Key 'a' already exists")
else:
    MyDic.Add ("a", "Aachen")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_Exists_IDictionary.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
