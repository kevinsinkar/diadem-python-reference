---
title: "ValueToChn"
description: "Possible spellings: ValueToChn, VariantToChn"
---

# ValueToChn

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ValueToChn

Possible spellings: ValueToChn, VariantToChn

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Write ValueToChn instead of VariantToChn.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SrcVariant</td>
<td>Specifies the name of the variant that DIAdem converts into channels.<div id="exp_SrcVariant">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ChnBaseName</td>
<td>Specifies the base name of the new channels, which is used when the channels are converted from an array.<div id="exp_ChnBaseName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[TransposeMatrix]</td>
<td>Specifies whether DIAdem transposes the matrix, which means DIAdem exchanges the rows and columns. The default value is <span class="Monospace">FALSE</span> which means that DIAdem does not swap the rows and columns.<div id="exp_TransposeMatrix">
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
<td>Specifies a channel list as a vector in the script environment. The return value is a ChannelList type.<div id="exp_ChannelList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
objVI.Run(True)
varArray = objVI.GetControlValue("OutPut1")
ChnLst = dd.ValueToChn(varArray,"DatafromLV")
# Clean up
objVI = NothingLVRuntime.DeInit
```

---

*Source: `ComOff/ValueToChn.htm`*
