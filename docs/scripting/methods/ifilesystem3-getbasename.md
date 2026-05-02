---
title: "IFileSystem3.GetBaseName"
description: "Returns the part of the path that corresponds with the filename of a file without filename extension."
---

# IFileSystem3.GetBaseName

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetBaseName for FileSystemObject

Returns the part of the path that corresponds with the filename of a file without filename extension.

## Signature

```python
sGetBaseName = Object.GetBaseName(Path)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def GetName(sFile):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    GetName = fso.GetBaseName(sFile)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetBaseName_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
