---
title: "PrinterName"
description: "Valid names: PrinterName, PrintName"
---

# PrinterName

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: PrinterName

Valid names: PrinterName, PrintName

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note </strong>If you use the DIAdem PDF printer, the last entry in this variable, which describes the port, must be "NUL", for example, "winspool,DIAdem PDF Export,NUL:".</td></tr></table>
</div>

## Python example

```python
dd.PrinterName = "winspool,\\\\National\\LJ5P,Ne02:"
```

---

*Source: `VarOff/PrinterName.htm`*
