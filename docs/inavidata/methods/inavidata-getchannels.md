---
title: "INaviData.GetChannels"
description: "Returns a collection of channels in the script interface for internal data. DIAdem sorts the result list in ascending channel number order. Use the GetChannels "
---

# INaviData.GetChannels

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: GetChannels for Data

Returns a collection of channels in the script interface for internal data. DIAdem sorts the result list in ascending channel number order. Use the GetChannels method to create data objects from channel references, for example, from layout configurations, and then to continue processing the data using the script interface for internal data.

## Signature

```python
return_value = obj.GetChannels(Reference)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Execute the <a href="../../../comoff/commands/chnrenumber/">ChnRenumber</a> command before using the <span class="Monospace">GetChannels</span> method, in order to align the channel sequence in the list with the channel sequence in the structure view. The <span class="Monospace">GetChannels</span> method always returns the list of channels in the global channel number sequence of DIAdem.</td></tr></table>
</div>

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Weather.tdm")
oMyChannels = dd.Data.GetChannels("Weather/T*")
for oMyChn in oMyChannels:
    sOutput = sOutput + "\r\n" + oMyChn.Name
print("Channel names: " + sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>Related Functions</h2><p class="Body"><a href="../inavidata-getchannel/">GetChannel</a> | <a href="../inavidata-getchannelgroups/">GetChannelGroups</a></p>
<h2>See Also</h2><p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_GetChannels_INaviData.HTM`*
