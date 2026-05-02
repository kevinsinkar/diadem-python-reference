---
title: "IFileSystem3"
description: "You can use the FileSystemObject object to access the file system of your computer. To use the FileSystemObject object, you must create this object in DIAdem wi"
---

# IFileSystem3

!!! abstract "Object &middot; `Scripting.chm`"
    Object: FileSystemObject

You can use the FileSystemObject object to access the file system of your computer. To use the FileSystemObject object, you must create this object in DIAdem with the CreateObject("Scripting.FileSystemObject") command.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
fso = win32com.client.Dispatch("Scripting.FileSystemObject")
MyFile= fso.CreateTextFile(ScriptWritePath + "\testfile.txt", True)
MyFile.WriteLine("This is the first line")
MyFile.Close
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ifilesystem3-drives/">Drives</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ifilesystem3-buildpath/">BuildPath</a> | <a href="../../methods/ifilesystem3-copyfile/">CopyFile</a> | <a href="../../methods/ifilesystem3-copyfolder/">CopyFolder</a> | <a href="../../methods/ifilesystem3-createfolder/">CreateFolder</a> | <a href="../../methods/ifilesystem3-createtextfile/">CreateTextFile</a> | <a href="../../methods/ifilesystem3-deletefile/">DeleteFile</a> | <a href="../../methods/ifilesystem3-deletefolder/">DeleteFolder</a> | <a href="../../methods/ifilesystem3-driveexists/">DriveExists</a> | <a href="../../methods/ifilesystem3-fileexists/">FileExists</a> | <a href="../../methods/ifilesystem3-folderexists/">FolderExists</a> | <a href="../../methods/ifilesystem3-getabsolutepathname/">GetAbsolutePathName</a> | <a href="../../methods/ifilesystem3-getbasename/">GetBaseName</a> | <a href="../../methods/ifilesystem3-getdrive/">GetDrive</a> | <a href="../../methods/ifilesystem3-getdrivename/">GetDriveName</a> | <a href="../../methods/ifilesystem3-getextensionname/">GetExtensionName</a> | <a href="../../methods/ifilesystem3-getfile/">GetFile</a> | <a href="../../methods/ifilesystem3-getfilename/">GetFileName</a> | <a href="../../methods/ifilesystem3-getfileversion/">GetFileVersion</a> | <a href="../../methods/ifilesystem3-getfolder/">GetFolder</a> | <a href="../../methods/ifilesystem3-getparentfoldername/">GetParentFolderName</a> | <a href="../../methods/ifilesystem3-getspecialfolder/">GetSpecialFolder</a> | <a href="../../methods/ifilesystem3-getstandardstream/">GetStandardStream</a> | <a href="../../methods/ifilesystem3-gettempname/">GetTempName</a> | <a href="../../methods/ifilesystem3-movefile/">MoveFile</a> | <a href="../../methods/ifilesystem3-movefolder/">MoveFolder</a> | <a href="../../methods/ifilesystem3-opentextfile/">OpenTextFile</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/objects/Scripting_Objects_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
