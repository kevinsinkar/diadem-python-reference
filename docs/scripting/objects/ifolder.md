---
title: "IFolder"
description: "You can use the Folder object to access the properties of a folder."
---

# IFolder

!!! abstract "Object &middot; `Scripting.chm`"
    Object: Folder

You can use the Folder object to access the properties of a folder.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowFolderInfo(sFolder):
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sFolder)
    sOutput = "Folder: " + oMyFolder.Name + VBCrLf
    sOutput = sOutput + "Created: " + oMyFolder.DateCreated + VBCrLf
    sOutput = sOutput + "Last Accessed: " + oMyFolder.DateLastAccessed + VBCrLf
    sOutput = sOutput + "Last Modified: " + oMyFolder.DateLastModified
    ShowFolderInfo = sOutput
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ifolder-attributes/">Attributes</a> | <a href="../../properties/ifolder-datecreated/">DateCreated</a> | <a href="../../properties/ifolder-datelastaccessed/">DateLastAccessed</a> | <a href="../../properties/ifolder-datelastmodified/">DateLastModified</a> | <a href="../../properties/ifolder-drive/">Drive</a> | <a href="../../properties/ifolder-files/">Files</a> | <a href="../../properties/ifolder-isrootfolder/">IsRootFolder</a> | <a href="../../properties/ifolder-name/">Name</a> | <a href="../../properties/ifolder-parentfolder/">ParentFolder</a> | <a href="../../properties/ifolder-path/">Path</a> | <a href="../../properties/ifolder-shortname/">ShortName</a> | <a href="../../properties/ifolder-shortpath/">ShortPath</a> | <a href="../../properties/ifolder-size/">Size</a> | <a href="../../properties/ifolder-subfolders/">SubFolders</a> | <a href="../../properties/ifolder-type/">Type</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ifolder-copy/">Copy</a> | <a href="../../methods/ifolder-createtextfile/">CreateTextFile</a> | <a href="../../methods/ifolder-delete/">Delete</a> | <a href="../../methods/ifolder-move/">Move</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idrive/">Drive</a>.<a href="../../properties/idrive-rootfolder/">RootFolder</a> | <a href="../ifile/">File</a>.<a href="../../properties/ifile-parentfolder/">ParentFolder</a> | <a href="../ifilesystem3/">FileSystemObject</a>.<a href="../../methods/ifilesystem3-createfolder/">CreateFolder</a> | <a href="../ifilesystem3/">FileSystemObject</a>.<a href="../../methods/ifilesystem3-getfolder/">GetFolder</a> | <a href="../ifilesystem3/">FileSystemObject</a>.<a href="../../methods/ifilesystem3-getspecialfolder/">GetSpecialFolder</a> | <a href="./">Folder</a>.<a href="../../properties/ifolder-parentfolder/">ParentFolder</a> | <a href="../../collections/folders/">Folders</a>.<a href="../../methods/ifoldercollection-add/">Add</a> | <a href="../../collections/folders/">Folders</a>.<a href="../../properties/ifoldercollection-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/objects/Scripting_Objects_IFolder.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
