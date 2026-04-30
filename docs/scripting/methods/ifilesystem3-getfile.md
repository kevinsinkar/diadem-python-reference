---
title: "IFileSystem3.GetFile"
description: "Returns a file object that is associated with a path."
---

# IFileSystem3.GetFile

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetFile for FileSystemObject

Returns a file object that is associated with a path.

## Signature

```python
return_value = obj.GetFile(FilePath)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def GetFileObject(sFile):
    fso = CreateObject("Scripting.FileSystemObject")
    GetFileObject = fso.GetFile(sFile)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetFile_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
