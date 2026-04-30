---
title: "IFileList.Add"
description: "Adds an element to a file list you drag to another object. You can use this method in the EventDragStart event in order to edit a file list."
---

# IFileList.Add

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Add for FileList  <DropInformation>

Adds an element to a file list you drag to another object. You can use this method in the EventDragStart event in order to edit a file list.

## Signature

```python
obj.Add(Value)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventDragStart(ByRef This, ByRef DropInformation, ByRef DropEffect):
    oMyFileList = DropInformation.FileList
    oMyFileList.RemoveAll
    oMyFileList.Add("C:\Test")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Add_IFileList.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
