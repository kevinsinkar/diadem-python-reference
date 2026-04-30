---
title: "BlChannelProperties"
description: "The channel properties object provides the methods and properties to set the channel properties which you can use in the DAC save block."
---

# BlChannelProperties

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: BlChannelProperties

The channel properties object provides the methods and properties to set the channel properties which you can use in the DAC save block.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="./image/note.gif"/></td><td><strong>Note  </strong>You must use the following object hierarchy to access the variable:<br attr="ext"/><br attr="ext"/>
<donottranslate><pre>Call DACObjOpen(<em>BlockName</em>)
    <em>Value</em> = BlChannelProperties(i)
Call DACObjClose(<em>BlockName</em>)</pre></donottranslate><br attr="ext"/>You need the DAC block name to open the DAC block, to access the variable, and to close the DAC block.<br attr="ext"/><br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td></tr></table>
</div>

## Python example

```python
import datetime
dd.DACObjOpen("Save1")
dd.BlGroupProperties.Add()
iCount=dd.BlGroupProperties.Count
dd.BlGroupProperties.Type(iCount)=dd.DataTypeFloat64
dd.BlGroupProperties.Name(iCount)="MyGroupProperty"
dd.BlGroupProperties.PropValue(iCount) = 1.234
for i in range( 1, dd.BlDataInpSigMax(1)+1):
    dd.BlChannelProperties(i).add()
    iCount=dd.BlChannelProperties(i).Count
    dd.BlChannelProperties(i).Type(iCount)=dd.DataTypeString
    dd.BlChannelProperties(i).Name(iCount)="MyChannelProperty"
    if dd.BlDataSourceName(i,1) == "Temperature" :
        dd.BlChannelProperties(i).PropValue(iCount) = "@@Monthname(month(datetime.datetime.now()))@@"
    else:
        dd.BlChannelProperties(i).PropValue(iCount) = "@@Weekdayname(weekday(datetime.datetime.now()))@@"
dd.DACObjClose("Save1")
```

---

*Source: `VarOnl/BlChannelProperties.htm`*
