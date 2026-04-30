---
title: "ExecuteExclusiveEnd"
description: "Ends the execution a mutually exclusive script section. If an instance is terminated, the execution of a mutually exclusive script section is automatically rele"
---

# ExecuteExclusiveEnd

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ExecuteExclusiveEnd

Ends the execution a mutually exclusive script section. If an instance is terminated, the execution of a mutually exclusive script section is automatically released to the other instances.

## Signature

```python
dd.ExecuteExclusiveEnd( ExecuteExclusiveHandle )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ExecuteExclusiveHandle</td>
<td>Specifies the handle for executing a mutually exclusive script section.<div id="exp_ExecuteExclusiveHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
intExecuteExclusiveHandle = dd.ExecuteExclusiveBegin("WriteFile",10)
if intExecuteExclusiveHandle < 0 :
    dd.DBM ("Timeout: Could not write file")
else:
    intMyFileHandle =  dd.TextFileOpen(dd.CurrentScriptPath + "MyFile.txt", dd.eTextFileAttributeExclusive or dd.eTextFileAttributeWrite or dd.eTextFileAttributeANSI)
    dd.TextFileWriteln(intMyFileHandle,"Test")
    intMyError = dd.TextFileClose(intMyFileHandle)
dd.ExecuteExclusiveEnd(intExecuteExclusiveHandle)
```

---

*Source: `ComOff/ExecuteExclusiveEnd.htm`*
