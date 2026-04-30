---
title: "IDictionary.Remove"
description: "Deletes a key/element pair from a Dictionary collection."
---

# IDictionary.Remove

!!! abstract "Method &middot; `Scripting.chm`"
    Method: Remove for Dictionary

Deletes a key/element pair from a Dictionary collection.

## Signature

```python
obj.Remove(Key)
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

# ... Further instructions

if MyDic.Exists("a"):
    MyDic.Remove ("a")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_Remove_IDictionary.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
