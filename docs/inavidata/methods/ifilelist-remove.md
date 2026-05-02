---
title: "IFileList.Remove"
description: "Deletes an element in a file list you drag to another object. You can use this method in the EventDragStart event in order to edit a file list."
---

# IFileList.Remove

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Remove for FileList  <DropInformation>

Deletes an element in a file list you drag to another object. You can use this method in the EventDragStart event in order to edit a file list.

## Signature

```python
obj.Remove(Index)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventDragStart(This, DropInformation, DropEffect):
    oMyFileList = DropInformation.FileList
    if oMyFileList.Count > 0:
        oMyFileList.Remove(oMyFileList.Count)
        oMyFileList.Add("C:\Test")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Remove_IFileList.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
