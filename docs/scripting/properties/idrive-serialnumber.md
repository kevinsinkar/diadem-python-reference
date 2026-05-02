---
title: "IDrive.SerialNumber"
description: "Specifies the unique decimal serial number of a drive."
---

# IDrive.SerialNumber

!!! abstract "Property &middot; `Scripting.chm`"
    Property: SerialNumber for Drive

Specifies the unique decimal serial number of a drive.

## Signature

```python
obj.SerialNumber
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateDriveSerialList():
    fso = CreateObject("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    for oMyDrive in oMyDrives:
        sOutput = sOutput + oMyDrive.DriveLetter + "\t"
        if oMyDrive.IsReady:
            sOutput = sOutput + oMyDrive.SerialNumber
        else:
            sOutput = sOutput + "[not ready]"
        sOutput = sOutput + "\r\n"
    CreateDriveSerialList = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/properties/Scripting_property_SerialNumber_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
