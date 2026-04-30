---
title: "LogfileBrowser"
description: "Opens the current DIAdem logfile in the editor."
---

# LogfileBrowser

!!! abstract "Command &middot; `ComOff.chm`"
    Command: LogfileBrowser

Opens the current DIAdem logfile in the editor.

## Signature

```python
dd.LogfileBrowser()
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You use the <a href="../../../varoff/variables/logfileeditname/">LogFileEditName</a> variable to specify the text editor for displaying and editing a logfile.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Python example

```python
dd.LogFileWrite("Testing")
dd.LogFileBrowser()
```

---

*Source: `ComOff/LogfileBrowser.htm`*
