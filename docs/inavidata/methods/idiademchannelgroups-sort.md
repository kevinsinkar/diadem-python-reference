---
title: "IDiademChannelGroups.Sort"
description: "Sorts the channel groups in the Data Portal alphabetically in the script interface for internal data."
---

# IDiademChannelGroups.Sort

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Sort for ChannelGroups <Data>

Sorts the channel groups in the Data Portal alphabetically in the script interface for internal data.

## Signature

```python
obj.Sort(Sorting)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSortAlphaAscending` | 1 | Alphabetically ascending |
| `eSortAlphaDescending` | 2 | Alphabetically descending |

## Python example

```python
oMyChannelGroups = dd.Data.Root.ChannelGroups
oMyChannelGroups.Sort(dd.eSortAlphaDescending)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Sort_IDiademChannelGroups.htm`*
