---
title: "IFile.Type"
description: "Specifies the type of a file."
---

# IFile.Type

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Type for File

Specifies the type of a file.

## Signature

```python
obj.Type
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowFileType(sFile):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    ShowFileType = oMyFile.Type
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Type_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
