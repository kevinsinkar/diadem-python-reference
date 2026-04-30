---
title: "IDiademUSIElement.IsKindOf"
description: "Checks the type of an element in the script interface for internal data."
---

# IDiademUSIElement.IsKindOf

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: IsKindOf for Element <Data>

Checks the type of an element in the script interface for internal data.

## Signature

```python
bIsKindOf = Object.IsKindOf(Type)
```

## Python example

```python
dd.MsgBoxDisp ("Please select one element in the Data Portal. Click 'interaction off' after selecting.")
dd.InteractionOn()
oMyElement = dd.Portal.ActiveView.Selection(1)
if oMyElement.IsKindOf(dd.eDataRoot) :
    dd.MsgBoxDisp ("Selected element: Root")
elif oMyElement.IsKindOf(dd.eDataChannelGroup) :
    dd.MsgBoxDisp ("Selected element: ChannelGroup")
elif oMyElement.IsKindOf(dd.eDataChannel) :
    dd.MsgBoxDisp ("Selected element: Channel")
```

```python
oMyElement = dd.Portal.ActiveView.Selection(1)
if oMyElement.IsKindOf(dd.eDataChannelWF) :
    dd.MsgBoxDisp("Property name: " + oMyElement.Properties("wf_xname").Value + "\r\n" + "Property unit: " + oMyElement.Properties("wf_xunit_string").Value)
else:
    dd.MsgBoxDisp ("Selected element is no waveform channel")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_IsKindOf_IDiademUSIElement.HTM`*
