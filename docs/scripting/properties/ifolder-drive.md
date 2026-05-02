---
title: "IFolder.Drive"
description: "Returns the Drive object for a folder. You can use this to access the associated drive."
---

# IFolder.Drive

!!! abstract "Property &middot; `Scripting.chm`"
    Property: Drive for Folder

Returns the Drive object for a folder. You can use this to access the associated drive.

## Signature

```python
return_value = obj.Drive
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def FolderDrive(sFolder):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    FolderDrive = "Drive: " + oMyFolder.Drive
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_Drive_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
