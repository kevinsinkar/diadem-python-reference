---
title: "HdCreate"
description: "Generates external channel headers."
---

# HdCreate

!!! abstract "Command &middot; `ComOff.chm`"
    Command: HdCreate

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.IntegerVarSet('GHdChnNo', ...)   # instead of dd.GHdChnNo = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Generates external channel headers.

## Signature

```python
dd.HdCreate()
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Python example

```python
dd.HdDelAll()
dd.GHdChnNo = 4
dd.GHdChnLength = 6
dd.GHdChnType = "EXPLICIT"
dd.GHdDispFormat= "Numeric"
dd.GHdChnFile = "MyFile.asc"
dd.GHdSaveType = "CHANNEL"
dd.GHdChnIdx = 4
dd.GHdChnMode = "ASCII"
dd.GHdAsciiPtr = 1
dd.GHdDecChar = "."
dd.GHdExChar = "E"
dd.GHdSep = ","
dd.GHdOffs = 0
dd.HdCreate()
dd.HdMarkAll()
dd.HdSave("MyFile")
```

---

*Source: `ComOff/HdCreate.htm`*
