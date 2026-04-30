---
title: "ChnAreaDel"
description: "Deletes values in a channel."
---

# ChnAreaDel

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnAreaDel

Deletes values in a channel.

## Signature

```python
dd.ChnAreaDel(ChnArg1, ChnRow, ValNo)
```

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
<p class="Body"><br attr="ext"/>If you use a channel number to specify a channel as text, note that the channels in the structure view of the Data Portal are not always in the same order as the channel numbers. <br attr="ext"/>For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.<br attr="ext"/>Refer to the <a href="#" data-unresolved="1">Channels and Channel References</a> page for more information about the various ways to clearly specify channels.</p>
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
</table>
</div>

## Python example

```python
dd.ChnAreaDel("Example/Time",1,10)
```

---

*Source: `ComOff/ChnAreaDel.htm`*
