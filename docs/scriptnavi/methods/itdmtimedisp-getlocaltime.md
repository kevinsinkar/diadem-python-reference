---
title: "ITDMTimeDisp.GetLocalTime"
description: "Returns the time information saved in the USITimeDisp object as local time. The local time consists of a date and time specification. The GetLocalTime method do"
---

# ITDMTimeDisp.GetLocalTime

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetLocalTime for UsiTimeDisp

Returns the time information saved in the USITimeDisp object as local time. The local time consists of a date and time specification. The GetLocalTime method does not execute a plausibility check and assumes that the time information to be converted is in UTC time. If this is not the case, the results are invalid. Therefore we recommend you know how local time is related to UTC time when you use this method. For example, UTC + 1 hour applies in Germany, which means 1 p. m. UTC is the same as 2 p.m. local time. During the daylight saving time, Germany adds a further hour to the UTC time.

## Signature

```python
return_value = obj.GetLocalTime()
```

## Python example

```python
UTC = dd.CreateTime(2014,4,25,14,35,10)
LocalTime = UTC.GetLocalTime()
dd.MsgBoxDisp(LocalTime.Hour + ":" + LocalTime.Minute + ":" + LocalTime.Second)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetLocalTime_ITDMTimeDisp.htm`*
