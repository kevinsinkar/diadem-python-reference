---
title: "INaviData.GetChannelGroups"
description: "Returns a collection of channel groups in the script interface for internal data."
---

# INaviData.GetChannelGroups

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: GetChannelGroups for Data

Returns a collection of channel groups in the script interface for internal data.

## Signature

```python
return_value = obj.GetChannelGroups(Reference)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If the method <span class="Monospace">GetChannelGroups</span> does not find a channel group that matches the specified criteria in the <span class="Monospace">Reference</span> parameter or if the expression is not valid, the method returns an empty list.</td></tr></table>
</div>

## Python example

```python
oMyChannelGroups = dd.Data.GetChannelgroups("[2,4,5..7],[]")
for oMyChnGrp in oMyChannelGroups:
    dd.MsgBoxDisp(oMyChnGrp.Name)
```

```python
oMyChannelGroups = dd.Data.GetChannelgroups("E*")
for oMyChnGrp in oMyChannelGroups:
    dd.MsgBoxDisp(oMyChnGrp.Name)
```

```python
oMyChannelGroups = dd.Data.GetChannelgroups("Example/Time,[2]")
for oMyChnGrp in oMyChannelGroups:
    dd.MsgBoxDisp(oMyChnGrp.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_GetChannelGroups_INaviData.htm`*
