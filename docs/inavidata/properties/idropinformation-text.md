---
title: "IDropInformation.Text"
description: "Specifies a text you drag and drop to a different object."
---

# IDropInformation.Text

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Text for DropInformation

Specifies a text you drag and drop to a different object.

## Signature

```python
obj.Text
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def XTable1_EventDrop(This, Row, Col, DropInformation):
    if DropInformation.IsKindOf(eDropText):
        Msgbox(DropInformation.Text)
    elif DropInformation.IsKindOf(eDropDataStoreElement):
        Msgbox(DropInformation.DataStoreElements.Count)

def XTable1_EventValGet(This, Row, Col, Cell, IsInputCell):
    Cell.Text = ""

def XTable1_EventDropAllowed(This, Row, Col, DropInformation, DropEffect):
    DropEffect = eDropEffectCopy
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Text_IDropInformation.htm`&nbsp;&middot;&nbsp;Python translated from VBS*
