---
title: "IFileSystem3.DeleteFile"
description: "Deletes one or more files."
---

# IFileSystem3.DeleteFile

!!! abstract "Method &middot; `Scripting.chm`"
    Method: DeleteFile for FileSystemObject

Deletes one or more files.

## Signature

```python
obj.DeleteFile(FileSpec, [Force])
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def DeleteMyFiles(sFile,bForce):
    fso = CreateObject("Scripting.FileSystemObject")
    fso.DeleteFile(sFile,bForce)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_DeleteFile_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
