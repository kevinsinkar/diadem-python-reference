---
title: "IDictionary.CompareMode"
description: "Specifies how a Dictionary collection compares text keys. By default, the Dictionary collection compares text."
---

# IDictionary.CompareMode

!!! abstract "Property &middot; `Scripting.chm`"
    Property: CompareMode for Dictionary

Specifies how a Dictionary collection compares text keys. By default, the Dictionary collection compares text.

## Signature

```python
obj.CompareMode
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Const BinaryCompare = 0
Const TextCompare = 1
MyDic = CreateObject("Scripting.Dictionary")
MyDic.CompareMode = BinaryCompare
MyDic.Add ("a", "Austin")
MyDic.Add ("A", "Aachen")
MyKeys = MyDic.Keys
for MyKey in MyKeys:
    sOutput = sOutput + MyKey + VBCrLf
dd.MsgBox(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_CompareMode_IDictionary.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
