---
title: "IFolder.Delete"
description: "Deletes a folder."
---

# IFolder.Delete

!!! abstract "Method &middot; `Scripting.chm`"
    Method: Delete for Folder

Deletes a folder.

## Signature

```python
obj.Delete([Force])
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def DeleteEntireFolder(sFolder,bForce):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    oMyFolder.Delete(bForce)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_Delete_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
