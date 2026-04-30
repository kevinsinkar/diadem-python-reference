---
title: "IFileSystem3.MoveFile"
description: "Moves one or more files."
---

# IFileSystem3.MoveFile

!!! abstract "Method &middot; `Scripting.chm`"
    Method: MoveFile for FileSystemObject

Moves one or more files.

## Signature

```python
obj.MoveFile(Source, Destination)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The MoveFile method aborts as soon as the first error occurs. DIAdem does not undo changes made to the file system before an error occurred.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def MoveFiles(sSource,sTarget):
    fso = CreateObject("Scripting.FileSystemObject")
    fso.MoveFile(sSource,sTarget)
MoveFiles("C:\Examples\Documents\*.tdr", "c:\Temp")
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_MoveFile_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
