---
title: "IFileList.Count"
description: "Specifies the number of elements in a file list which you drag and drop onto another object."
---

# IFileList.Count

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Count for FileList  <DropInformation>

Specifies the number of elements in a file list which you drag and drop onto another object.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def Tree1_EventDropAllowed(This, DropInformation, DropEffect):  # Created Event Handler
    if (DropInformation.FileList.Count >0):
        DropEffect = eDropEffectCopy

def Tree1_EventDrop(This, DropInformation, DropEffect, Node):
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

*Source: `Inavidata/properties/DiaCmpnt_property_Count_IFileList.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
