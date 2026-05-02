---
title: "IFileList.Item"
description: "Returns in a file list that you drag and drop to another object the file or folder associated with a specific index."
---

# IFileList.Item

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Item for FileList  <DropInformation>

Returns in a file list that you drag and drop to another object the file or folder associated with a specific index.

## Signature

```python
sItem = Object.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> property because it is the standard element of the collection.</td>
</tr>
</table>
</div>

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

## Members

<div markdown="1">
<div class="Properties"><h2> </h2>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Item_IFileList.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
