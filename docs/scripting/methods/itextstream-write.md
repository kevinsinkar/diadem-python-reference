---
title: "ITextStream.Write"
description: "Writes a text into a TextStream file."
---

# ITextStream.Write

!!! abstract "Method &middot; `Scripting.chm`"
    Method: Write for TextStream

Writes a text into a TextStream file.

## Signature

```python
obj.Write(Text)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def CreateTxtFile(sFile,sText):
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.CreateTextFile(sFile, True)
    oMyFile.Write(sText)
    oMyFile.Close
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_Write_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
