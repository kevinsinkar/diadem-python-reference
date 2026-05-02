---
title: "PrinterName"
description: "Valid names: PrinterName, PrintName"
---

# PrinterName

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: PrinterName

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('PrinterName', ...)   # instead of dd.PrinterName = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

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
