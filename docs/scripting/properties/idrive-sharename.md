---
title: "IDrive.ShareName"
description: "Returns the release name of a drive."
---

# IDrive.ShareName

!!! abstract "Property &middot; `Scripting.chm`"
    Property: ShareName for Drive

Returns the release name of a drive.

## Signature

```python
obj.ShareName
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def DriveInfo(sDrv):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyDrive = fso.GetDrive(fso.GetDriveName(fso.GetAbsolutePathName(sDrv)))
    DriveInfo = "Drive: " + oMyDrive.DriveLetter + VBCrLf + "Shared name: " + oMyDrive.ShareName
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_ShareName_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
