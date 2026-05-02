---
title: "IDictionary.RemoveAll"
description: "Deletes all key/element pairs from a Dictionary collection."
---

# IDictionary.RemoveAll

!!! abstract "Method &middot; `Scripting.chm`"
    Method: RemoveAll for Dictionary

Deletes all key/element pairs from a Dictionary collection.

## Signature

```python
obj.RemoveAll
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
MyDic.RemoveAll
MyKeys = MyDic.Keys
for MyKey in MyKeys:
    sOutput = sOutput + MyKey + "\r\n"
dd.MsgBox(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_RemoveAll_IDictionary.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
