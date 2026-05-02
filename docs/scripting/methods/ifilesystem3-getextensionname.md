---
title: "IFileSystem3.GetExtensionName"
description: "Returns the part of the path that corresponds with the filename extension of a file."
---

# IFileSystem3.GetExtensionName

!!! abstract "Method &middot; `Scripting.chm`"
    Method: GetExtensionName for FileSystemObject

Returns the part of the path that corresponds with the filename extension of a file.

## Signature

```python
sGetExtensionName = Object.GetExtensionName(Path)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def GetExtension(sDrive):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    GetExtension = fso.GetExtensionName(sDrive)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_GetExtensionName_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
