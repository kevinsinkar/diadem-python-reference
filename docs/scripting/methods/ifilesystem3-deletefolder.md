---
title: "IFileSystem3.DeleteFolder"
description: "Deletes a folder and its content."
---

# IFileSystem3.DeleteFolder

!!! abstract "Method &middot; `Scripting.chm`"
    Method: DeleteFolder for FileSystemObject

Deletes a folder and its content.

## Signature

```python
obj.DeleteFolder(FolderSpec, [Force])
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def DeleteMyFolder(sFile):
    fso = CreateObject("Scripting.FileSystemObject")
    fso.DeleteFolder(sFile)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_DeleteFolder_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
