---
title: "ChnSRTMAltitude"
description: "Determines the corresponding elevation values from the latitudes and longitudes. Before calling this function, you must download the appropriate SRTM data into "
---

# ChnSRTMAltitude

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSRTMAltitude

Determines the corresponding elevation values from the latitudes and longitudes. Before calling this function, you must download the appropriate SRTM data into the cache folder using the SRTMDownloadTilesArea function.

## Signature

```python
return_value = dd.ChnSRTMAltitude( X , Y , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies data channel containing the latitudes.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the longitudes.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel names. If you do not specify the name, DIAdem creates the <span class="Monospace">AltitudeSRTM</span> channel in the default group.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel with the elevation values. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnSRTMAltitude.htm`*
