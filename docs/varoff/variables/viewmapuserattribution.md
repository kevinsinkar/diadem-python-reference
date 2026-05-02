---
title: "VIEWMapUserAttribution"
description: "Specifies the copyright of the map provider."
---

# VIEWMapUserAttribution

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: VIEWMapUserAttribution

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('VIEWMapUserURL', ...)   # instead of dd.VIEWMapUserURL = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Specifies the copyright of the map provider.

## Python example

```python
dd.VIEWMapUserURL="http://192.168.228.129/tile/{z}/{x}/{y}.png"
dd.VIEWMapUsermaxZoom=20
dd.VIEWMapUserAttribution="(c) OpenStreetMap (and) contributors, CC-BY-SA"
```

---

*Source: `VarOff/VIEWMapUserAttribution.htm`*
