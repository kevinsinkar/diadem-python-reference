---
title: "IFileSystem3.BuildPath"
description: "Adds a name to a path."
---

# IFileSystem3.BuildPath

!!! abstract "Method &middot; `Scripting.chm`"
    Method: BuildPath for FileSystemObject

Adds a name to a path.

## Signature

```python
sBuildPath = Object.BuildPath(Path, Name)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def BuildNewPath(sPath):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    BuildNewPath = fso.BuildPath(sPath, "NewFolder")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_BuildPath_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
