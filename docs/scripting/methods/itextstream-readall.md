---
title: "ITextStream.ReadAll"
description: "Reads in all of the TextStream file."
---

# ITextStream.ReadAll

!!! abstract "Method &middot; `Scripting.chm`"
    Method: ReadAll for TextStream

Reads in all of the TextStream file.

## Signature

```python
sReadAll = Object.ReadAll
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ReadFile(sFile):
    ForReading = 1
    fso = win32com.client.Dispatch("Scripting.FileSystemObject")
    oMyFile = fso.OpenTextFile(sFile, ForReading, False)
    ReadFile = oMyFile.ReadAll
    oMyFile.Close
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `Scripting/methods/Scripting_method_ReadAll_ITextStream.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
