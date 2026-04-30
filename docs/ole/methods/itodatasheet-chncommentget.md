---
title: "ITODataSheet.ChnCommentGet"
description: "Reads a channel comment."
---

# ITODataSheet.ChnCommentGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnCommentGet for TODataSheet

Reads a channel comment.

## Signature

```python
iChnCommentGet = Object.ChnCommentGet(vChnV, vCommentP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ChnCommentGet("Time",vCommentP)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnCommentGet_ITODataSheet.htm`*
