---
title: "IFolder.ShortPath"
description: "Specifies the short path of a folder according to the 8.3 naming convention."
---

# IFolder.ShortPath

!!! abstract "Property &middot; `Scripting.chm`"
    Property: ShortPath for Folder

Specifies the short path of a folder according to the 8.3 naming convention.

## Signature

```python
obj.ShortPath
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FolderShortPath(sFolder):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    FolderShortPath = "Shortpath: " + oMyFolder.ShortPath
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_ShortPath_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
