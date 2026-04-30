---
title: "IAssignment.DefinitionRange"
description: "Specifies the value range of a channel to which a specific text value is assigned, in the script interface for internal data. A text value (property Value ) is "
---

# IAssignment.DefinitionRange

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: DefinitionRange for Assignment <Data>

Specifies the value range of a channel to which a specific text value is assigned, in the script interface for internal data. A text value (property Value ) is assigned to a numeric value (property Definition ) or to a value range (property DefinitionRange ) in order to define an assignment.

## Signature

```python
obj.DefinitionRange
```

## Python example

```python
grp = dd.Data.Root.ChannelGroups(1)
chn = grp.Channels.AddAssignmentChannel("MyAssignmentChn", "Default Value", dd.DataTypeChnFloat64, 1)
asgn_list = chn.AssignmentList
asgn_list.Add("text1", [10, 20])
asgn_list.Add("text2", [30, 40])
asgn_list.Add("text3", [50, 60])
for assignment in asgn_list:
    range = assignment.DefinitionRange
    print("Definition Range", range[0], "-", range[1], ":", assignment.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_DefinitionRange_IAssignment.htm`*
