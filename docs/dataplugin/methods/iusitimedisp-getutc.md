---
title: "IUsiTimeDisp.GetUTC"
description: "Returns the time information saved in the USITimeDisp object in coordinated world time as UTC time (Universal Time Coordinated). UTC time consists of a date and"
---

# IUsiTimeDisp.GetUTC

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: GetUTC for UsiTimeDisp

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Returns the time information saved in the USITimeDisp object in coordinated world time as UTC time (Universal Time Coordinated). UTC time consists of a date and time specification. The GetUTC method does not execute a plausibility check and assumes that the time information to be converted is in local time. If this is not the case, the results are invalid. Therefore we recommend you know how local time is related to UTC time when you use this method. For example, UTC + 1 hour applies in Germany, which means 1 p. m. UTC is the same as 2 p.m. local time. During the daylight saving time, Germany adds a further hour to the UTC time.

## Signature

```python
return_value = obj.GetUTC
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
MsgBoxDisp(UTC.Hour + ":" + UTC.Minute + ":" + UTC.Second)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_GetUTC_IUsiTimeDisp.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
