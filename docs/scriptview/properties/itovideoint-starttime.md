---
title: "IToVideoInt.StartTime"
description: "Specifies the time delay of a video in DIAdem VIEW.  If you use a video channel to select the video, you cannot change the FrameRate and the StartTime propertie"
---

# IToVideoInt.StartTime

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: StartTime for Video

Specifies the time delay of a video in DIAdem VIEW.  If you use a video channel to select the video, you cannot change the FrameRate and the StartTime properties. DIAdem then determines the frame rate and the start time from the corresponding properties of the video channel or, if these channel properties have the NoValue value, DIAdem determines the settings from the video file. If you change the path of the video file in the script by using the channel property NI_Video~file , the frame rate by using the channel property NI_Video~frame_rate , or the start time of the video channel by using the channel property NI_Video~start_time , you must call the Refresh method so that DIAdem recalculates the frame rate and start time for the video in VIEW.

## Signature

```python
obj.StartTime
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "Video"
oMyObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyObj.FileName = dd.ProgramDrv  + "\\Examples\\Documents\\Austin_Drive.wmv"
oMyObj.FrameRate = 25
oMyObj.StartTime = 0
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_StartTime_IToVideoInt.htm`*
