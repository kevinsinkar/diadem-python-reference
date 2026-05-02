---
title: "IImplicitChannel.Values"
description: "Contains the single value of a channel at a specific channel position."
---

# IImplicitChannel.Values

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Values for ImplicitChannel

Contains the single value of a channel at a specific channel position.

## Signature

```python
obj.Values(iIndex)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  The <span class="Monospace">Size</span> property contains the current number of values of a channel.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyChn = Root.ChannelGroup(1).Channels(1)
if (oMyChn.IsKindOf(eDataImplicitChannel)):
    MsgBoxDisp("Channel name: " + oMyChn.Name + "\r\n" + "First value: " + oMyChn.Values(1))
else:
    MsgBoxDisp("No implicit channel")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Values_IImplicitChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
