---
title: "IFile.Delete"
description: "Deletes a file."
---

# IFile.Delete

!!! abstract "Method &middot; `Scripting.chm`"
    Method: Delete for File

Deletes a file.

## Signature

```python
obj.Delete([Force])
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def DeleteMyFile(sFile,bForce):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    oMyFile.Delete(bForce)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_Delete_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
