---
title: "DocStart"
description: "Starts a print job."
---

# DocStart

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DocStart

Starts a print job.

## Signature

```python
dd.DocStart()
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Python example

```python
dd.DocStart()
dd.Report.LoadLayout("Report1")
dd.Report.Refresh()
dd.Report.ActiveSheet.Print()
dd.Report.LoadLayout("Report2")
dd.Report.Refresh()
dd.Report.ActiveSheet.Print()
dd.DocEnd()
```

---

*Source: `ComOff/DocStart.htm`*
