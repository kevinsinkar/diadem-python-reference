---
title: "ExecuteExclusiveBegin"
description: "Starts the execution of a script section with mutual exclusion (mutex). Another program instance, which also starts the execution of a mutually exclusive script"
---

# ExecuteExclusiveBegin

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ExecuteExclusiveBegin

Starts the execution of a script section with mutual exclusion (mutex). Another program instance, which also starts the execution of a mutually exclusive script section for which it uses the same name, will wait for the first instance to finish the execution of the script section. You create a mutual exclusion by inserting the critical script lines into the ExecuteExclusiveBegin and ExecuteExclusiveEnd commands. Use these commands, for example, for parallel processes with multiple Worker objects or within SystemLink TDM to access files exclusively.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ExecuteExclusiveName</td>
<td>Specifies the name for executing a mutually exclusive script section.<div id="exp_ExecuteExclusiveName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum 200 characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[ExecuteExclusiveTimeout]</td>
<td>Specifies the time in seconds that DIAdem waits for the execution of a mutually exclusive script section. If you specify a negative value, DIAdem waits for another instance to release the execution of a mutually exclusive script section.<div id="exp_ExecuteExclusiveTimeout">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>-1 &lt;= ExecuteExclusiveTimeout &lt;= 10000<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Specifies the handle that DIAdem returns when executing a mutually exclusive script section. If the handle is smaller than <span class="Monospace">0</span>, another instance executes a mutually exclusive script section and has not yet released execution.<div id="exp_ExecuteExclusiveHandle">
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

*Source: `ComOff/ExecuteExclusiveBegin.htm`*
