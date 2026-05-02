---
title: "IFile.Path"
description: "Specifies the path of a file."
---

# IFile.Path

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Path for File

Specifies the path of a file.

## Signature

```python
obj.Path
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FilePath(sFile):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    FilePath = "Path: " + oMyFile.Path
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Path_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
