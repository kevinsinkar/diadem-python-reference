---
title: "VIEWMapUserMaxZoom"
description: "Specifies the maximum zoom level of the map server."
---

# VIEWMapUserMaxZoom

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: VIEWMapUserMaxZoom

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('VIEWMapUserURL', ...)   # instead of dd.VIEWMapUserURL = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Specifies the maximum zoom level of the map server.

## Python example

```python
dd.VIEWMapUserURL="https://tile.thunderforest.com/cycle/{z}/{x}/{y}.png?apikey="
dd.VIEWMapUsermaxZoom=22
dd.VIEWMapUserAttribution="Maps © Thunderforest, Data © OpenStreetMap contributors"
```

---

*Source: `VarOff/VIEWMapUserMaxZoom.htm`*
