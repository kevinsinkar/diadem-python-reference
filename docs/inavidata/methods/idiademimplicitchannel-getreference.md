---
title: "IDiademImplicitChannel.GetReference"
description: "Returns the channel reference of an implicit channel in the script interface for internal data."
---

# IDiademImplicitChannel.GetReference

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: GetReference for ImplicitChannel <Data>

Returns the channel reference of an implicit channel in the script interface for internal data.

## Signature

```python
sGetReference = Object.GetReference(ReferenceType)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eReferenceDefault` | 0 | Channel reference of the DIAdem setting |
| `eReferenceNameName` | 1 | Group name/Channel name |
| `eReferenceIndexName` | 2 | [Group index]/Channel name |
| `eReferenceNameIndex` | 3 | Group name/[Channel index] |
| `eReferenceIndexIndex` | 4 | [Group index]/[Channel index] |

## Python example

```python
oMyImplChannel = dd.Data.Root.ActiveChannelGroup.Channels(1)
if oMyImplChannel.IsKindOf(dd.eDataImplicitChannel) :
    dd.MsgBoxDisp(oMyImplChannel.GetReference(dd.ExtendChnName))
else:
    dd.MsgBoxDisp("No implicit channel")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_GetReference_IDiademImplicitChannel.htm`*
