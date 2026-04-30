---
title: "UIAutoRefreshSet"
description: "Specifies whether DIAdem informs the Data Portal and the DIAdem VIEW panel about changes to the channel contents or the channel properties while the program is "
---

# UIAutoRefreshSet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: UIAutoRefreshSet

Specifies whether DIAdem informs the Data Portal and the DIAdem VIEW panel about changes to the channel contents or the channel properties while the program is running a script.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you enable the refresh function, you decrease the <a href="#" data-unresolved="1">processing speed</a>. If you switch off Data Portal refresh during debugging using the <span class="Monospace">UIAutoRefreshSet</span> command, errors can occur because the Data Portal does not always display the actual data.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">UIAutoRefreshArg</td>
<td>Specifies whether DIAdem informs the Data Portal and the DIAdem VIEW panel about changes to the channel contents or the channel properties. If the variable has the value <span class="Monospace">TRUE</span>, DIAdem refreshes the Data Portal and the DIAdem VIEW panel.<div id="exp_UIAutoRefreshArg">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean variable</a> type. The return value contains the refresh behavior that was set before the <span class="Monospace">UIAutoRefreshSet</span> executed.</td></tr>
</table>
</div>

## Python example

```python
import math
#Script faster
MyTimeStart = Timer
dd.UIAutoRefreshSet(False) #Switch refresh off
dd.ChnLinGen("/Gen_temp",1,2*math.pi,100000,"rad") #Generate temporary channel
dd.Calculate("Ch(\"Grp/Sinus\") = Sin(Ch(\"/Gen_temp\"))" ) #Calculate sinus channel
dd.Data.Root.ActiveChannelGroup.Channels.Remove("Gen_temp") #Delete temporary channel
MyTimeEnd = Timer
dd.UIAutoRefreshSet(False) #Switch refresh off
dd.MsgBoxDisp(MyTimeEnd-MyTimeStart)

#Script slower
MyTimeStart = Timer
dd.UIAutoRefreshSet(True) #Switch refresh on
dd.ChnLinGen("/Gen_temp",1,2*math.pi,100000,"rad") #Generate temporary channel
dd.Calculate("Ch(\"Grp/Sinus\") = Sin(Ch(\"/Gen_temp\"))" ) #Calculate sinus channel
dd.Data.Root.ActiveChannelGroup.Channels.Remove("Gen_temp") #Delete temporary channel
MyTimeEnd = Timer
dd.UIAutoRefreshSet(False) #Switch refresh off
dd.MsgBoxDisp(MyTimeEnd-MyTimeStart)
```

---

*Source: `ComOff/UIAutoRefreshSet.htm`*
