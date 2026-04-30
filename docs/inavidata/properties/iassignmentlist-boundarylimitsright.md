---
title: "IAssignmentList.BoundaryLimitsRight"
description: "Specifies the interval limit of the maximum value of an assignment in an assignment channel in the script interface for internal data."
---

# IAssignmentList.BoundaryLimitsRight

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: BoundaryLimitsRight for AssignmentList <Data>

Specifies the interval limit of the maximum value of an assignment in an assignment channel in the script interface for internal data.

## Signature

```python
obj.BoundaryLimitsRight
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>   Specify the interval limits in a script before you generate individual assignments.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you define assignments with single values, use the <span class="Monospace">BoundsClose</span> setting for the minimum and the maximum.</td></tr></table>
</div>

## Python example

```python
# Function to convert Boundary Limits from integer into text
def LimitAsText(limit_type):
    result = "unknown"
    if (limit_type == dd.BoundsOpen):
        result = "BoundsOpen"
    elif (limit_type == dd.BoundsClose):
        result = "BoundsClose"
    return result

chn = dd.Data.Root.ChannelGroups(1).Channels.AddAssignmentChannel("MyAssignmentChn", "Default Value")
asgn_list = chn.AssignmentList
asgn_list.SetBoundaryLimits(dd.BoundsOpen, dd.BoundsClose)
asgn_list.Add("text1", [10, 20])
asgn_list.Add("text2", [20, 30])
asgn_list.Add("text3", [30, 40])
print("Left Limits:", LimitAsText(asgn_list.BoundaryLimitsLeft))
print("Right Limits:", LimitAsText(asgn_list.BoundaryLimitsRight))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_BoundaryLimitsRight_IAssignmentList.htm`*
