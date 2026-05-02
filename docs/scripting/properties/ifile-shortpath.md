---
title: "IFile.ShortPath"
description: "Specifies the short path according to the 8.3 naming convention."
---

# IFile.ShortPath

!!! abstract "Property &middot; `Scripting.chm`"
    Property: ShortPath for File

Specifies the short path according to the 8.3 naming convention.

## Signature

```python
obj.ShortPath
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FileShortPath(sFile):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    FileShortPath = "Shortpath: " + oMyFile.ShortPath
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_ShortPath_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
