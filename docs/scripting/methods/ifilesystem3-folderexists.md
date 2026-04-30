---
title: "IFileSystem3.FolderExists"
description: "Checks whether a folder exists"
---

# IFileSystem3.FolderExists

!!! abstract "Method &middot; `Scripting.chm`"
    Method: FolderExists for FileSystemObject

Checks whether a folder exists

## Signature

```python
bFolderExists = Object.FolderExists(FolderSpec)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FolderStatus(sFolder):
    fso = CreateObject("Scripting.FileSystemObject")
    if (fso.FolderExists(sFolder)):
        sOutput = sFolder + " exists."
    else:
        sOutput = sFolder + " doesn't exist."
    FolderStatus = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_FolderExists_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
