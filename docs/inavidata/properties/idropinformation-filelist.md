---
title: "IDropInformation.FileList"
description: "Returns in user dialog boxes a collection of all files from a file list which you drag and drop to another object."
---

# IDropInformation.FileList

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: FileList for DropInformation

Returns in user dialog boxes a collection of all files from a file list which you drag and drop to another object.

## Signature

```python
return_value = obj.FileList
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Sub Tree1_EventDropAllowed(ByRef This, DropInformation, ByRef DropEffect) 'Created Event Handler
if (DropInformation.FileList.Count >0):
    DropEffect = eDropEffectCopy

def Tree1_EventDrop(ByRef This, DropInformation, ByRef DropEffect, ByRef Node):
    oMyFileList = DropInformation.FileList
    if (oMyFileList.Count > 0):
        if (not Node Is None):
            for iCount in range(1, oMyFileList.Count + 1):
                Node.Nodes.Add(oMyFileList(iCount))
            Node.Expanded = True
            Node.Update(eUpdateModeNodeAndChilds)
        else:
            for iCount in range(1, oMyFileList.Count + 1):
                This.Nodes.Add(oMyFileList(iCount))
            This.Refresh
    else:
        DropEffect = eDropEffectNone
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_FileList_IDropInformation.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
