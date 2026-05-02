---
title: "IFile"
description: "You can use the File object to access the properties of a file."
---

# IFile

!!! abstract "Object &middot; `Scripting.chm`"
    Object: File

You can use the File object to access the properties of a file.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ShowFileInfo(sFile):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.GetFile(sFile)
    sOutput = "File: " + oMyFile.Name + "\r\n"
    sOutput = sOutput + "Created: " + oMyFile.DateCreated + "\r\n"
    sOutput = sOutput + "Last Accessed: " + oMyFile.DateLastAccessed + "\r\n"
    sOutput = sOutput + "Last Modified: " + oMyFile.DateLastModified
    ShowFileInfo = sOutput
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ifile-attributes/">Attributes</a> | <a href="../../properties/ifile-datecreated/">DateCreated</a> | <a href="../../properties/ifile-datelastaccessed/">DateLastAccessed</a> | <a href="../../properties/ifile-datelastmodified/">DateLastModified</a> | <a href="../../properties/ifile-drive/">Drive</a> | <a href="../../properties/ifile-name/">Name</a> | <a href="../../properties/ifile-parentfolder/">ParentFolder</a> | <a href="../../properties/ifile-path/">Path</a> | <a href="../../properties/ifile-shortname/">ShortName</a> | <a href="../../properties/ifile-shortpath/">ShortPath</a> | <a href="../../properties/ifile-size/">Size</a> | <a href="../../properties/ifile-type/">Type</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ifile-copy/">Copy</a> | <a href="../../methods/ifile-delete/">Delete</a> | <a href="../../methods/ifile-move/">Move</a> | <a href="../../methods/ifile-openastextstream/">OpenAsTextStream</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/files/">Files</a>.<a href="../../properties/ifilecollection-item/">Item</a> | <a href="../ifilesystem3/">FileSystemObject</a>.<a href="../../methods/ifilesystem3-getfile/">GetFile</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/objects/Scripting_Objects_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
