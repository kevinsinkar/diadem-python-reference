---
title: "SRTMDownloadTilesArea"
description: "Downloads SRTM data for the specified area into the cache folder. The SRTM data contains a high-resolution digital terrain model of the earth surface with the e"
---

# SRTMDownloadTilesArea

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SRTMDownloadTilesArea (Obsolete)

Downloads SRTM data for the specified area into the cache folder. The SRTM data contains a high-resolution digital terrain model of the earth surface with the elevation value for nearly every position on the earth. Use the SRTMDownloadGetStatistics function to get statistical data on the downloaded data.

## Signature

```python
dd.SRTMDownloadTilesArea(SRTMLowerLatitudeBound, SRTMUpperLatitudeBound, SRTMLowerLongitudeBound, SRTMUpperLongitudeBound)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note </strong>This command is obsolete.<br attr="ext"/>Use the example <a href="#" data-unresolved="1">Searching for Obsolete Commands and Variables</a> to search for outdated commands and variables in your scripts.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>To download SRTM data to the cache folder, you need to login first. To do this, register at <span class="Monospace">https://urs.earthdata.nasa.gov/users/new</span> and specify the user name via the variable <a href="../../../varoff/variables/srtmusername/">SRTMUsername</a> and the password via <a href="../../../varoff/variables/srtmpassword/">SRTMPassword</a>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SRTMLowerLatitudeBound</td>
<td>Specifies the lower latitude limit.<div id="exp_SRTMLowerLatitudeBound">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMUpperLatitudeBound</td>
<td>Specifies the upper latitude limit.<div id="exp_SRTMUpperLatitudeBound">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMLowerLongitudeBound</td>
<td>Specifies the lower longitude limit.<div id="exp_SRTMLowerLongitudeBound">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRTMUpperLongitudeBound</td>
<td>Specifies the upper longitude limit.<div id="exp_SRTMUpperLongitudeBound">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/SRTMDownloadTilesArea.htm`*
