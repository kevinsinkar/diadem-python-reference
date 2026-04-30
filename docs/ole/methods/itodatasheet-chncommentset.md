---
title: "ITODataSheet.ChnCommentSet"
description: "Sets a channel comment."
---

# ITODataSheet.ChnCommentSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnCommentSet for TODataSheet

Sets a channel comment.

## Signature

```python
iChnCommentSet = Object.ChnCommentSet(vChnV, sgCommentV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ChnCommentSet("Time","Comment")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnCommentSet_ITODataSheet.htm`*
