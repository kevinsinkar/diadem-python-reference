---
title: "IFile.ShortName"
description: "Specifies the short name of a file according to the 8.3 naming convention."
---

# IFile.ShortName

!!! abstract "Property &middot; `Scripting.chm`"
    Property: ShortName for File

Specifies the short name of a file according to the 8.3 naming convention.

## Signature

```python
obj.ShortName
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FileShortName(sFile):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    FileShortName = "Shortname: " + oMyFile.ShortName
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_ShortName_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
