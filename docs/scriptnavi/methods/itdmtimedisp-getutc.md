---
title: "ITDMTimeDisp.GetUTC"
description: "Returns the time information saved in the USITimeDisp object in coordinated world time as UTC time (Universal Time Coordinated). UTC time consists of a date and"
---

# ITDMTimeDisp.GetUTC

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetUTC for UsiTimeDisp

Returns the time information saved in the USITimeDisp object in coordinated world time as UTC time (Universal Time Coordinated). UTC time consists of a date and time specification. The GetUTC method does not execute a plausibility check and assumes that the time information to be converted is in local time. If this is not the case, the results are invalid. Therefore we recommend you know how local time is related to UTC time when you use this method. For example, UTC + 1 hour applies in Germany, which means 1 p. m. UTC is the same as 2 p.m. local time. During the daylight saving time, Germany adds a further hour to the UTC time.

## Signature

```python
return_value = obj.GetUTC()
```

## Python example

```python
LocalTime = dd.CreateTime(2014,4,25,14,35,10)
UTC = LocalTime.GetUTC()
dd.MsgBoxDisp(UTC.Hour + ":" + UTC.Minute + ":" + UTC.Second)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetUTC_ITDMTimeDisp.htm`*
