---
title: "PartToReserve"
description: "Specifies the percentage of messages at the end of a logfile, which DIAdem does not delete when it resets."
---

# PartToReserve

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: PartToReserve

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.IntegerVarSet('PartToReserve', ...)   # instead of dd.PartToReserve = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Specifies the percentage of messages at the end of a logfile, which DIAdem does not delete when it resets.

## Python example

```python
dd.PartToReserve  =  10
dd.LogFileReset   = 200
dd.LogfileBrowser()
```

---

*Source: `VarOff/PartToReserve.htm`*
