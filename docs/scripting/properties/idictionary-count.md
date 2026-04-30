---
title: "IDictionary.Count"
description: "Counts all key/element pairs from a Dictionary collection."
---

# IDictionary.Count

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Count for Dictionary

Counts all key/element pairs from a Dictionary collection.

## Signature

```python
obj.Count
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
MyKeys = MyDic.Keys
for i in range(0, MyDic.Count-1 + 1):
    sOutput = sOutput + MyKeys(i) + VBCrLf
dd.MsgBox(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Count_IDictionary.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
