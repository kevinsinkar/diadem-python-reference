---
title: "ITextStream.ReadLine"
description: "Reads a text file line of a TextStream file up to the end of line identifier."
---

# ITextStream.ReadLine

!!! abstract "Method &middot; `Scripting.chm`"
    Method: ReadLine for TextStream

Reads a text file line of a TextStream file up to the end of line identifier.

## Signature

```python
sReadLine = Object.ReadLine
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ReadFile(sFile):
    Const ForReading = 1
    fso = CreateObject("Scripting.FileSystemObject")
    oMyFile = fso.OpenTextFile(sFile, ForReading, False)
    while oMyFile.AtEndOfStream != True:
        sOutput = sOutput + oMyFile.ReadLine + VBCrLf
    oMyFile.Close
    ReadFile = sOutput
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_ReadLine_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
