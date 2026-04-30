---
title: "IFileSystem3.MoveFolder"
description: "Moves one or more folders."
---

# IFileSystem3.MoveFolder

!!! abstract "Method &middot; `Scripting.chm`"
    Method: MoveFolder for FileSystemObject

Moves one or more folders.

## Signature

```python
obj.MoveFolder(Source, Destination)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The MoveFolder method aborts as soon as the first error occurs. DIAdem does not undo changes made to the file system before an error occurred.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def MoveEntireFolder(sSource,sTarget):
    fso = CreateObject("Scripting.FileSystemObject")
    fso.MoveFolder(sSource,sTarget)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_MoveFolder_IFileSystem3.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
