---
title: "Drives"
description: "A collection of all Drive objects. You can count drives or access an individual drive using the Drives collection."
---

# Drives

!!! abstract "Collection &middot; `Scripting.chm`"
    Collection: Drives

A collection of all Drive objects. You can count drives or access an individual drive using the Drives collection.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateDriveList():
    fso = CreateObject("Scripting.FileSystemObject")
    oMyDrives = fso.Drives
    for oMyDrive in oMyDrives:
        sOutput = sOutput + oMyDrive.DriveLetter + VBTab
        if oMyDrive.DriveType = 3:
            sOutput = sOutput + oMyDrive.ShareName
            ElseIf oMyDrive.IsReady :
            sOutput = sOutput + oMyDrive.VolumeName
        else:
            sOutput = sOutput + "[not ready]"
        sOutput = sOutput + VBCrLf
    CreateDriveList = sOutput
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idrivecollection-count/">Count</a> | <a href="../../properties/idrivecollection-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/ifilesystem3/">FileSystemObject</a>.<a href="../../properties/ifilesystem3-drives/">Drives</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/objects/Scripting_Objects_IDriveCollection.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
