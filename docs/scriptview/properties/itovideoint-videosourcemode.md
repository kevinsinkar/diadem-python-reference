---
title: "IToVideoInt.VideoSourceMode"
description: "Specifies whether DIAdem displays a video file or a video channel in a video in DIAdem VIEW. By default, DIAdem uses a video file. Use the SetVideo for Video me"
---

# IToVideoInt.VideoSourceMode

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: VideoSourceMode for Video

Specifies whether DIAdem displays a video file or a video channel in a video in DIAdem VIEW. By default, DIAdem uses a video file. Use the SetVideo for Video method to specify whether DIAdem uses a video file or a video channel and to specify the name with path of the video file or the channel reference of the video channel.

## Signature

```python
obj.VideoSourceMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eVideoFile` | 0 | Video file |
| `eVideoChannel` | 1 | Video channel |

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "Video"
oMyObj = oMySheet.ActiveArea.DisplayObj
oMyObj.VideoSourceMode = dd.eVideoFile
oMyObj.FileName = dd.ProgramDrv + "Examples\\Documents\\Plate.avi"
oMyObj.FrameRate = 50
oMyObj.Sound = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Alignment Functions in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Automatic Display of Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Bird's Eye View Display</a> | <a href="#" data-unresolved="1">Calculating a Tangent to a Curve</a> | <a href="#" data-unresolved="1">Contour Display in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Creating and Viewing Long Data Channels</a> | <a href="#" data-unresolved="1">Dynamic Display of Statistical Characteristic Values in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Overlaying Objects in Videos</a> | <a href="#" data-unresolved="1">Planetary Motion</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Data</a> | <a href="#" data-unresolved="1">Synchronizing Videos and Waveform Data</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">Using a User Command to Calculate the Difference between the Y-Values</a> | <a href="#" data-unresolved="1">Various Display Modes in DIAdem VIEW</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a> | <a href="#" data-unresolved="1">Viewing and Automatically Analyzing Data</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_VideoSourceMode_IToVideoInt.htm`*
