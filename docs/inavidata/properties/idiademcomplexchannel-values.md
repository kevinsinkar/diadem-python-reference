---
title: "IDiademComplexChannel.Values"
description: "Specifies the single value of a complex channel at a specific channel position in the script interface for internal data."
---

# IDiademComplexChannel.Values

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Values for ComplexChannel <Data>

Specifies the single value of a complex channel at a specific channel position in the script interface for internal data.

## Signature

```python
obj.Values(Index)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Values</span> property because this property is a standard element of the object. To access the first value of the first channel, you can use the following notation:<pre><donottranslate>
Set oMyChannel = Data.Root.ActiveChannelGroup.Channels(1)
oMyValue = oMyChannel.Values(1)</donottranslate></pre>
<br attr="ext"/>The following notation is also possible.<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>oMyValue = oMyChannel(1)</donottranslate></pre><br attr="ext"/>If you do not specify the <span class="Monospace">Values</span> property and use an object variable for the channel object, you accelerate access to the values of the channel.</td></tr></table>
</div>

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups.Add("MyChnGroup")
oMyChn = oMyGrp.Channels.Add("MyChannel", dd.DataTypeFloat64)
for i in range( 1, 100+1):
    oMyChn = []
oMyChn.append(float(i/100000))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Values_IDiademComplexChannel.htm`*
