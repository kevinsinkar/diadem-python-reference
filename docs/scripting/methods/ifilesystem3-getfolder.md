---
title: "IFileSystem3.GetFolder"
description: "Returns a folder object belonging to a path."
---

# IFileSystem3.GetFolder

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetFolder for FileSystemObject

Returns a folder object belonging to a path.

## Signature

```python
return_value = obj.GetFolder(FolderPath)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def GetFolderObject(sFolder):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    GetFolderObject = fso.GetFolder(sFolder)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetFolder_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
