---
title: "IDiademChannels.AddVideoChannel"
description: "Generates a new video channel in the script interface for internal data."
---

# IDiademChannels.AddVideoChannel

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: AddVideoChannel for Channels <Data>

Generates a new video channel in the script interface for internal data.

## Signature

```python
return_value = obj.AddVideoChannel(Name, File, FilePathMode, [FrameRate], [StartTime], [DestIndex])
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eFilePathRelative` | 1 | Relative path to the data file |
| `eFilePathAbsolute` | 2 | Absolute path |

## Python example

```python
oMyVideoChn= dd.Data.Root.ChannelGroups(1).Channels.AddVideoChannel("Video", "Safetytest02.wmv", dd.eFilePathRelative,dd.NoValue, dd.NoValue, 1)
dd.MsgBoxDisp(oMyVideoChn.GetReference(dd.ExtendChnName))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_AddVideoChannel_IDiademChannels.htm`*
