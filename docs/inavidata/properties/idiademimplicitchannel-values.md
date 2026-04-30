---
title: "IDiademImplicitChannel.Values"
description: "Specifies the single value of an implicit channel at a specific channel position in the script interface for internal data. The property Size specifies the numb"
---

# IDiademImplicitChannel.Values

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Values for ImplicitChannel <Data>

Specifies the single value of an implicit channel at a specific channel position in the script interface for internal data. The property Size specifies the number of values in an implicit channel.

## Signature

```python
obj.Values(Index)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><ul><li>The <strong>Values</strong> property returns a value of the <span class="Monospace">VBDate</span> data type. This data type has a valid range from 01/01/100 to 31/12/9999 23:59:59. On 30/12/1899 you can only use time information but no date information. If you convert <span class="Monospace">VBDate</span> type values that contain only time information into the USITimeDisp format, the program automatically adds the <span class="Monospace">01/01/0000</span> date information. If you convert <span class="Monospace">VBDate</span> type values into the DIAdem time format, the program adds the date information in relation to the variable <a href="../../../varoff/variables/applicationtimebasehighresolution/">ApplicationTimebaseHighResolution</a>.</li>
<li>The <strong>oValues</strong> property supplies time values as <a href="../../../scriptnavi/objects/itdmtimedisp/">USITimeDisp object</a> in the USITimeDisp format. Use the <span class="Monospace">oValues</span> property if you are working with time values that lie within the range between January 1 of the year zero and 01/01/100, or concern December 30 1899. The USITimeDisp object is valid from 01/01 of the year zero to 12/31/9999 23:59:59.</li>
<li>The property <strong>dValues</strong> provides time values as double values in the DIAdem time format in relation to the variable <a href="../../../varoff/variables/applicationtimebasehighresolution/">ApplicationTimebaseHighResolution</a>. Use the <span class="Monospace">dValues</span> property if you are working with time values that lie within the range between January 1 of the year zero and 01/01/100, or concern December 30 1899. The DIAdem time format is valid from 01/01 of the year zero to 12/31/9999 23:59:59.</li></ul></td></tr></table>
</div>

## Python example

```python
oMyChn = dd.Data.Root.ActiveChannelGroup.Channels(1)
if (oMyChn.IsKindOf(dd.eDataImplicitChannel)) :
    dd.MsgBoxDisp("Channel name: " + oMyChn.Name + "\r\n" + "First value: " + oMyChn.Values(1))
else:
    dd.MsgBoxDisp("No implicit channel")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Values_IDiademImplicitChannel.htm`*
