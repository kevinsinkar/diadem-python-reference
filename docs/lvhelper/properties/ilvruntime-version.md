---
title: "ILVRuntime.Version"
description: "Returns the LabVIEW version that the LVRuntime uses."
---

# ILVRuntime.Version

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: Version for LVRuntime

Returns the LabVIEW version that the LVRuntime uses.

## Signature

```python
obj.Version
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  You can omit the <span class="Monospace">Version</span> property because the property is a standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
dd.MsgBoxDisp (dd.LVRuntime.Version)
dd.LVRuntime.DeInit()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/properties/LVHelper_property_Version_ILVRuntime.htm`*
