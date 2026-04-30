---
title: "IDiademProperties.Exists"
description: "Checks whether a Property object with a specific name already exists in the properties collection in the script interface for internal data."
---

# IDiademProperties.Exists

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Exists for Properties <Data>

Checks whether a Property object with a specific name already exists in the properties collection in the script interface for internal data.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
if dd.Data.Root.Properties.Exists("TimeBegin") :
    dd.Data.Root.Properties.Add("TimeEnd", dd.CurrTime)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Exists_IDiademProperties.HTM`*
