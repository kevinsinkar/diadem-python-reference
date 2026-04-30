---
title: "ExecuteExclusiveEndAll"
description: "Ends all executions of mutually exclusive script sections.  If an instance is terminated, the execution of a mutually exclusive script section is automatically "
---

# ExecuteExclusiveEndAll

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ExecuteExclusiveEndAll

Ends all executions of mutually exclusive script sections.  If an instance is terminated, the execution of a mutually exclusive script section is automatically released to the other instances.

## Signature

```python
dd.ExecuteExclusiveEndAll()
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
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
dd.ExecuteExclusiveEndAll()
```

---

*Source: `ComOff/ExecuteExclusiveEndAll.htm`*
