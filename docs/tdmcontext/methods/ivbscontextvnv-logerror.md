---
title: "IVbsContextVnV.LogError"
description: "Creates an error. The data preparation continues the script but marks the file in the data preparation as failed."
---

# IVbsContextVnV.LogError

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: LogError for ContextVnV <Data Preprocessor>

Creates an error. The data preparation continues the script but marks the file in the data preparation as failed.

## Signature

```python
obj.LogError(message)
```

## Python example

```python
def On_ValidationAndVerification(oContext):
    if dd.Data.GetChannels("*").Count == 0 :
        oContext.LogError("No data")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_LogError_IVbsContextVnV.htm`*
