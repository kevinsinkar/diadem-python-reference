---
title: "IDiademAssignmentChannel.UnitSymbol"
description: "Specifies the unit symbol of an assignment channel. The value of the UnitSymbol property for AssignmentChannel corresponds to the value of Object .Properties(\"u"
---

# IDiademAssignmentChannel.UnitSymbol

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: UnitSymbol for AssignmentChannel <Data>

Specifies the unit symbol of an assignment channel. The value of the UnitSymbol property for AssignmentChannel corresponds to the value of Object .Properties("unit_string").value .

## Signature

```python
obj.UnitSymbol
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\Report_expl.tdm")
oMyChn = dd.Data.GetChannel("[6]/[4]")
dd.MsgBoxDisp(oMyChn.UnitSymbol) # equivalent to oMyChn.Properties("unit_string").Value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_UnitSymbol_IDiademAssignmentChannel.htm`*
