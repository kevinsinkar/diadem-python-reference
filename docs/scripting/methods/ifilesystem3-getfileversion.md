---
title: "IFileSystem3.GetFileVersion"
description: "Specifies the version number of a file."
---

# IFileSystem3.GetFileVersion

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetFileVersion for FileSystemObject

Specifies the version number of a file.

## Signature

```python
sGetFileVersion = Object.GetFileVersion(FileName)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FileVersion(sFile):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    FileVersion = fso.GetFileVersion(sFile)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetFileVersion_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
