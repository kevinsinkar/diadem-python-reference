---
title: "StopWatchReset"
description: "Restarts a time measurement."
---

# StopWatchReset

!!! abstract "Command &middot; `ComOff.chm`"
    Command: StopWatchReset

Restarts a time measurement.

## Signature

```python
dd.StopWatchReset([StopWatchNo])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">[StopWatchNo]</td>
<td>Specifies the number of the time measurement. You can start several time measurements simultaneously. The default value of the <span class="Monospace">StopWatchNo</span> variable is <span class="Monospace">0</span>.<div id="exp_StopWatchNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150">StopWatch</td><td>Receives the time that has elapsed since the last start, in seconds.<div id="exp_StopWatch">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a><br attr="ext"/>i = 1 ... 5</td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr></table>
</div>

## Python example

```python
dd.StopWatchReset(1)
dd.ChnSmooth(1,"Smooth", 10, "maxNumber")
dd.MsgBoxDisp("Total time: "+dd.Str(dd.Stopwatch(1),"d.dddddd")+" Sec")
```

---

*Source: `ComOff/StopWatchReset.htm`*
