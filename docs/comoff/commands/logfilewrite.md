---
title: "LogfileWrite"
description: "Valid names: LogfileWrite, Print"
---

# LogfileWrite

!!! abstract "Command &middot; `ComOff.chm`"
    Command: LogfileWrite

Valid names: LogfileWrite, Print

## Signature

```python
dd.LogfileWrite( LogfileLine )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">LogfileLine</td>
<td>Specifies the text that DIAdem writes into a text file.<div id="exp_LogfileLine">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.LogFileWrite("Testing")
dd.LogFileBrowser()
```

---

*Source: `ComOff/LogfileWrite.htm`*
