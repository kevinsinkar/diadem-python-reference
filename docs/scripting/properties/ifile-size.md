---
title: "IFile.Size"
description: "Specifies the size of a file."
---

# IFile.Size

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Size for File

Specifies the size of a file.

## Signature

```python
obj.Size
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowFileSize(sFile):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    ShowFileSize = "Size: " + oMyFile.Size
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Size_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
