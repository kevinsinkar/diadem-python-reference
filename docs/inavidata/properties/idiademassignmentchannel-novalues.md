---
title: "IDiademAssignmentChannel.NoValues"
description: "Specifies whether a channel contains NoValues."
---

# IDiademAssignmentChannel.NoValues

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: NoValues for AssignmentChannel <Data>

Specifies whether a channel contains NoValues.

## Signature

```python
obj.NoValues
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  The <span class="Monospace">NoValues</span> property for <span class="Monospace">AssignmentChannel</span> returns the Boolean values <span class="Monospace">-1</span>, <span class="Monospace">0</span>, and <span class="Monospace">1</span>. If you use the <em><span class="Monospace">Object</span></em><span class="Monospace">.Properties("novaluekey").value</span> syntax to determine the value of the same property, DIAdem returns the text <span class="Monospace">Yes</span>, <span class="Monospace">No</span>, and <span class="Monospace">not calculated</span>.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eTriStateFalse` | 0 | No NoValues |
| `eTriStateUnknown` | 1 | Unknown |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\Report_expl.tdm")
oMyChn = dd.Data.GetChannel("[6]/[4]")
dd.MsgBoxDisp(oMyChn.NoValues) # equivalent to oMyChn.Properties("novaluekey").Value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_NoValues_IDiademAssignmentChannel.htm`*
