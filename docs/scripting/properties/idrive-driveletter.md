---
title: "IDrive.DriveLetter"
description: "Returns the drive letter of a drive."
---

# IDrive.DriveLetter

!!! abstract "Property &middot; `Scripting.chm`"
    Property: DriveLetter for Drive

Returns the drive letter of a drive.

## Signature

```python
obj.DriveLetter
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateDriveSpaceList():
    fso = CreateObject("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    for oMyDrive in oMyDrives:
        sOutput = sOutput + oMyDrive.DriveLetter + VBTab
        if oMyDrive.IsReady:
            sOutput = sOutput + FormatNumber(oMyDrive.FreeSpace,0)
        else:
            sOutput = sOutput + "[not ready]"
        sOutput = sOutput + VBCrLf
    CreateDriveSpaceList = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_DriveLetter_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
