---
title: "IDrive.RootFolder"
description: "Returns the Folder object of the root folder of a drive."
---

# IDrive.RootFolder

!!! abstract "Property &middot; `Scripting.chm`"
    Property: RootFolder for Drive

Returns the Folder object of the root folder of a drive.

## Signature

```python
return_value = obj.RootFolder
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def RootPath(sDrv):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyDrive = fso.GetDrive(fso.GetDriveName(fso.GetAbsolutePathName(sDrv)))
    RootPath = "Root: " + oMyDrive.RootFolder.Path
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_RootFolder_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
