---
title: "IDiademChannel.Values"
description: "Specifies the single value of a channel at a specific channel position in the script interface for internal data."
---

# IDiademChannel.Values

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Values for Channel <Data>

Specifies the single value of a channel at a specific channel position in the script interface for internal data.

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
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  When working with date values, pay attention to the following characteristics:<br attr="ext"/><br attr="ext"/><ul><li>The <strong>Values</strong> property returns a value of the <span class="Monospace">VBDate</span> data type. This data type has a valid range from 01/01/100 to 31/12/9999 23:59:59. On 30/12/1899 you can only use time information but no date information. If you convert <span class="Monospace">VBDate</span> type values that contain only time information into the USITimeDisp format, the program automatically adds the <span class="Monospace">01/01/0000</span> date information. If you convert <span class="Monospace">VBDate</span> type values into the DIAdem time format, the program adds the date information in relation to the variable <a href="../../../varoff/variables/applicationtimebasehighresolution/">ApplicationTimebaseHighResolution</a>.</li>
<li>The <strong>oValues</strong> property supplies time values as <a href="../../../scriptnavi/objects/itdmtimedisp/">USITimeDisp object</a> in the USITimeDisp format. Use the <span class="Monospace">oValues</span> property if you are working with time values that lie within the range between January 1 of the year zero and 01/01/100, or concern December 30 1899. The USITimeDisp object is valid from 01/01 of the year zero to 12/31/9999 23:59:59.</li>
<li>The property <strong>dValues</strong> provides time values as double values in the DIAdem time format in relation to the variable <a href="../../../varoff/variables/applicationtimebasehighresolution/">ApplicationTimebaseHighResolution</a>. Use the <span class="Monospace">dValues</span> property if you are working with time values that lie within the range between January 1 of the year zero and 01/01/100, or concern December 30 1899. The DIAdem time format is valid from 01/01 of the year zero to 12/31/9999 23:59:59.</li></ul></td></tr></table>
</div>

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups.Add("MyChnGroup")
oMyChn = oMyGrp.Channels.Add("MyChannel", dd.DataTypeFloat64)
for i in range( 1, 100+1):
    oMyChn = []
oMyChn.append(float(i/100000))
```

```python
oChn = dd.ChnGenTime("[1]/TimeGenerated", "second", dd.TTR("19.02.2021 11:05:01.0000", "#dd.mm.yyyy hh:nn:ss.ffff"), 0, 1, "StartStepNo", 200)
print (dd.RTT(oChn(1).dValues(oChn(1).Size), "#hh:nn:ss"))
```

```python
def ShowUsiTimeObj(oUsiTime):
    sHelpT = str(oUsiTime.Day) + "." + str(oUsiTime.Month) + "." + str(oUsiTime.Year)
    sHelpT = sHelpT + " -- "
    sHelpT = sHelpT + str(oUsiTime.Hour) + ":" + str(oUsiTime.Minute) + ":" + str(oUsiTime.Second)
    ShowUsiTimeObj = sHelpT
    return ShowUsiTimeObj

oChn = dd.Data.Root.ChannelGroups.Add("Test").Channels.Add("Time",dd.DataTypeDate)
oChn.dValues[1] = dd.TTR("30.07.2009 12:45:30", "#dd.mm.yyyy hh:nn:ss")
oChn.Values[2] = dd.CreateTime(2009, 7, 30, 12, 45, 30)
for Index in range( 1, 2+1):
    dd.LogfileWrite("DIAdem Date/Time (DoubleValue): " + dd.RTT(oChn.dValues( Index ), "#dd.mm.yyyy"))
    dd.LogfileWrite("DIAdem Date/Time (Object): "      + ShowUsiTimeObj (oChn.oValues( Index )))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Values_IDiademChannel.HTM`*
