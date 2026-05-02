---
title: "IFile.Copy"
description: "Copies a file to a different folder or to another file."
---

# IFile.Copy

!!! abstract "Method &middot; `Scripting.chm`"
    Method: Copy for File

Copies a file to a different folder or to another file.

## Signature

```python
obj.Copy(Destination, [OverWriteFiles])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The copy method aborts as soon as the first error occurs. DIAdem does not undo changes made to the file system before an error occurred.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CopyMyFiles(sSource,sTarget,bOverwrite):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFolder = fso.GetFolder(sSource)
    oMyFiles = oMyFolder.Files
    for oMyFile in oMyFiles:
        oMyFile.Copy(sTarget,bOverwrite)
CopyMyFiles(dd.ProgramDrv + "Examples\Documents\", "c:\Temp\Documents\",True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_Copy_IFile.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
