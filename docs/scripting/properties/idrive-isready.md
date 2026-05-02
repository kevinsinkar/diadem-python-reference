---
title: "IDrive.IsReady"
description: "Checks whether a drive is ready."
---

# IDrive.IsReady

!!! abstract "Property &middot; `Scripting.chm`"
    Property: IsReady for Drive

Checks whether a drive is ready.

## Signature

```python
obj.IsReady
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateDriveSpaceList():
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    for oMyDrive in oMyDrives:
        sOutput = sOutput + oMyDrive.DriveLetter + "\t"
        if oMyDrive.IsReady:
            sOutput = sOutput + FormatNumber(oMyDrive.FreeSpace,0)
        else:
            sOutput = sOutput + "[not ready]"
        sOutput = sOutput + "\r\n"
    CreateDriveSpaceList = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_IsReady_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
