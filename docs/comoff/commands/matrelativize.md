---
title: "MatRelativize"
description: "Determines for each element of a matrix the percentage the element has of the total sum of all matrix elements."
---

# MatRelativize

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatRelativize

Determines for each element of a matrix the percentage the element has of the total sum of all matrix elements.

## Signature

```python
dd.MatRelativize(ChnList, MatRelIP)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">MatRelIP</td>
<td>Specifies whether DIAdem overwrites the values of the input channels with the result values of the relativization.<div id="exp_MatRelIP">
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
oMyChannelList = dd.Data.GetChannels("Grp/ChnZ*")
dd.MatRelativize(oMyChannelList, True)
```

---

*Source: `ComOff/MatRelativize.htm`*
