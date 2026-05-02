---
title: "IFolder.ShortName"
description: "Specifies the short name according to the 8.3 naming convention."
---

# IFolder.ShortName

!!! abstract "Property &middot; `Scripting.chm`"
    Property: ShortName for Folder

Specifies the short name according to the 8.3 naming convention.

## Signature

```python
obj.ShortName
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FolderShortName(sFolder):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    FolderShortName = "Shortname: " + oMyFolder.ShortName
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_ShortName_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
