---
title: "IUsiTimeDisp.GetLocalTime"
description: "Returns the time information saved in the USITimeDisp object as local time. The local time consists of a date and time specification. The GetLocalTime method do"
---

# IUsiTimeDisp.GetLocalTime

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: GetLocalTime for UsiTimeDisp

Returns the time information saved in the USITimeDisp object as local time. The local time consists of a date and time specification. The GetLocalTime method does not execute a plausibility check and assumes that the time information to be converted is in UTC time. If this is not the case, the results are invalid. Therefore we recommend you know how local time is related to UTC time when you use this method. For example, UTC + 1 hour applies in Germany, which means 1 p. m. UTC is the same as 2 p.m. local time. During the daylight saving time, Germany adds a further hour to the UTC time.

## Signature

```python
return_value = obj.GetLocalTime
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
MsgBoxDisp(LocalTime.Hour + ":" + LocalTime.Minute + ":" + LocalTime.Second)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_GetLocalTime_IUsiTimeDisp.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
