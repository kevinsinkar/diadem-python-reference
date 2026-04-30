---
title: "IFile.Attributes"
description: "Specifies the attributes of a file."
---

# IFile.Attributes

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Attributes for File

Specifies the attributes of a file.

## Signature

```python
obj.Attributes
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def MakeWritable(sFile):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    if oMyFile.Attributes and 1:
        oMyFile.Attributes = oMyFile.Attributes - 1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Attributes_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
