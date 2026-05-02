---
title: "ASCIIOrdLength"
description: "Specifies the minimum length for ordinal numbers in ASCII block storage."
---

# ASCIIOrdLength

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ASCIIOrdLength

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.IntegerVarSet('ASCIIOrdLength', ...)   # instead of dd.ASCIIOrdLength = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Specifies the minimum length for ordinal numbers in ASCII block storage.

## Python example

```python
dd.ASCIIOrdLength = 5
MyNumber = 100 #  100'
MyNumber = 9 #    9'
dd.ASCIIOrdLength = 2
MyNumber = 103 #103'
```

---

*Source: `VarOff/ASCIIOrdLength.htm`*
