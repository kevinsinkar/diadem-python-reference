---
title: "IDrive"
description: "You can use the Drive object to access the properties of a drive."
---

# IDrive

!!! abstract "Object &middot; `Scripting.chm`"
    Object: Drive

You can use the Drive object to access the properties of a drive.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idrive-availablespace/">AvailableSpace</a> | <a href="../../properties/idrive-driveletter/">DriveLetter</a> | <a href="../../properties/idrive-drivetype/">DriveType</a> | <a href="../../properties/idrive-filesystem/">FileSystem</a> | <a href="../../properties/idrive-freespace/">FreeSpace</a> | <a href="../../properties/idrive-isready/">IsReady</a> | <a href="../../properties/idrive-path/">Path</a> | <a href="../../properties/idrive-rootfolder/">RootFolder</a> | <a href="../../properties/idrive-serialnumber/">SerialNumber</a> | <a href="../../properties/idrive-sharename/">ShareName</a> | <a href="../../properties/idrive-totalsize/">TotalSize</a> | <a href="../../properties/idrive-volumename/">VolumeName</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/drives/">Drives</a>.<a href="../../properties/idrivecollection-item/">Item</a> | <a href="../ifile/">File</a>.<a href="../../properties/ifile-drive/">Drive</a> | <a href="../ifilesystem3/">FileSystemObject</a>.<a href="../../methods/ifilesystem3-getdrive/">GetDrive</a> | <a href="../ifolder/">Folder</a>.<a href="../../properties/ifolder-drive/">Drive</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/objects/Scripting_Objects_IDrive.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
