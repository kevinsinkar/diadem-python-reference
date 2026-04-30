---
title: "MatNormalize"
description: "Normalizes the elements of a matrix to the maximum value one."
---

# MatNormalize

!!! abstract "Command &middot; `ComOff.chm`"
    Command: MatNormalize

Normalizes the elements of a matrix to the maximum value one.

## Signature

```python
dd.MatNormalize(ChnList, MatNormIP)
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
<tr><td width="150">MatNormIP</td>
<td>Specifies whether DIAdem overwrites the values of the input channels with the result values from the normalizing.<div id="exp_MatNormIP">
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
dd.MatNormalize(oMyChannelList, True)
```

---

*Source: `ComOff/MatNormalize.htm`*
