---
title: "DocEnd"
description: "Closes the document and sends the print job to the printer."
---

# DocEnd

!!! abstract "Command &middot; `ComOff.chm`"
    Command: DocEnd

Closes the document and sends the print job to the printer.

## Signature

```python
dd.DocEnd()
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

*Source: `ComOff/DocEnd.htm`*
