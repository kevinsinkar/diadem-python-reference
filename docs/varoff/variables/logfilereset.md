---
title: "LogfileReset"
description: "Specifies the maximum number of messages that DIAdem records in a logfile. When the logfile exceeds this number, DIAdem deletes all messages in the logfile."
---

# LogfileReset

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: LogfileReset

Specifies the maximum number of messages that DIAdem records in a logfile. When the logfile exceeds this number, DIAdem deletes all messages in the logfile.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Use the <a href="../parttoreserve/">PartToReserve</a> variable to specify which percentage of the messages DIAdem does not delete at the end of the logfile.</td></tr></table>
</div>

## Python example

```python
dd.PartToReserve  =  10
dd.LogFileReset   = 200
dd.LogfileBrowser()
```

---

*Source: `VarOff/LogfileReset.htm`*
