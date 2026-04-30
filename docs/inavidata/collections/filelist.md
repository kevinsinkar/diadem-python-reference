---
title: "FileList"
description: "Specifies a file list you drag and drop to a different object."
---

# FileList

!!! abstract "Collection &middot; `Inavidata.chm`"
    Collection: FileList  <DropInformation>

Specifies a file list you drag and drop to a different object.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Sub Tree1_EventDropAllowed(ByRef This, DropInformation, ByRef DropEffect) 'Creataed Event Handler
if (DropInformation.FileList.Count >0):
    DropEffect = eDropEffectCopy

def Tree1_EventDrop(ByRef This, DropInformation, ByRef DropEffect, ByRef Node):
    if (DropInformation.FileList.Count >0):
        if (not Node Is None):
            for oMyFile in DropInformation.FileList:
                Node.Nodes.Add(oMyFile)
            Node.Expanded = True
            Node.Update(eUpdateModeNodeAndChilds)
        else:
            for oMyFile in DropInformation.FileList:
                This.Nodes.Add(oMyFile)
            This.Refresh
    else:
        DropEffect = eDropEffectNone
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ifilelist-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ifilelist-add/">Add</a> | <a href="../../methods/ifilelist-item/">Item</a> | <a href="../../methods/ifilelist-remove/">Remove</a> | <a href="../../methods/ifilelist-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idropinformation/">DropInformation</a>.<a href="../../properties/idropinformation-filelist/">FileList</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IFileList.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
