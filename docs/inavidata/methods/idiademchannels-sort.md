---
title: "IDiademChannels.Sort"
description: "Sorts the channels of a channel group in the Data Portal alphabetically in the script interface for internal data."
---

# IDiademChannels.Sort

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Sort for Channels <Data>

Sorts the channels of a channel group in the Data Portal alphabetically in the script interface for internal data.

## Signature

```python
obj.Sort(Sorting, [UseChnXRelations])
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSortAlphaAscending` | 1 | Alphabetically ascending |
| `eSortAlphaDescending` | 2 | Alphabetically descending |

## Python example

```python
oMyChannels = dd.Data.Root.ChannelGroups(1).Channels
oMyChannels.Sort(dd.eSortAlphaAscending, True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Sort_IDiademChannels.htm`*
