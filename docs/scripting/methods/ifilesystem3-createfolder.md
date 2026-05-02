---
title: "IFileSystem3.CreateFolder"
description: "Creates a folder."
---

# IFileSystem3.CreateFolder

!!! abstract "Method &middot; `Scripting.chm`"
    Method: CreateFolder for FileSystemObject

Creates a folder.

## Signature

```python
return_value = obj.CreateFolder(Path)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateFolderObject(sFolder):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    CreateFolderObject = fso.CreateFolder(sFolder)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_CreateFolder_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
