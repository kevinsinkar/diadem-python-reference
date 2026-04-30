---
title: "IFileSystem3.GetParentFolderName"
description: "Returns the name of the superordinate folder for a file or a folder."
---

# IFileSystem3.GetParentFolderName

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetParentFolderName for FileSystemObject

Returns the name of the superordinate folder for a file or a folder.

## Signature

```python
sGetParentFolderName = Object.GetParentFolderName(Path)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ParentName(sDriveSpec):
    fso = CreateObject("Scripting.FileSystemObject")
    ParentName = fso.GetParentFolderName(sDriveSpec)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetParentFolderName_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
