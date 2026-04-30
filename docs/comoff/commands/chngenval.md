---
title: "ChnGenVal"
description: "Generates a data channel with equidistant values."
---

# ChnGenVal

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnGenVal

Generates a data channel with equidistant values.

## Signature

```python
dd.ChnGenVal(ChnArg1, ChnRow, ValNo, ChnBegin, ChnStep, [ValueOverwrite])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Use the commands <a href="../chnlingen/">ChnLinGen</a>, <a href="../chngeogen/">ChnGeoGen</a>, and <a href="../chndxdivgen/">ChnDXDivGen</a>, to generate channels in a script. Use the <a href="../chnlingenimp/">ChnLinGenImp</a> command to generate implicit channels.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnArg1</td>
<td>Specifies a channel.<div id="exp_ChnArg1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body">A channel is a <a href="../../../inavidata/objects/idiademchannel/">channel object</a> or a text, which relates to an individual channel.<br attr="ext"/>If you use a channel number to specify a channel as text, note that the channels in the structure view of the Data Portal are not always in the same order as the channel numbers. <br attr="ext"/>For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.<br attr="ext"/>Refer to the <a href="#" data-unresolved="1">Channels and Channel References</a> page for more information about the various ways to clearly specify channels.</p>
</div></td></tr>
<tr><td width="150">ChnRow</td>
<td>Specifies the row number in a channel.<div id="exp_ChnRow">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= ChnRow &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
<tr><td width="150">ValNo</td>
<td>Specifies the number of values in a channel.<div id="exp_ValNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= ValNo &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
<tr><td width="150">ChnBegin</td>
<td>Specifies the start value when DIAdem generates a channel.<div id="exp_ChnBegin">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ChnStep</td>
<td>Specifies the step width for generating equidistant channel values.<div id="exp_ChnStep">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ValueOverwrite]</td>
<td>Specifies whether DIAdem overwrites existing channel data. The default value is <span class="Monospace">FALSE</span>, which specifies that DIAdem does not overwrite the input channels.<div id="exp_ValueOverwrite">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.ChnGenVal("Grp/Chn3",1,100,0,2,0)
```

---

*Source: `ComOff/ChnGenVal.htm`*
