---
title: "IVbsContextASDeinit.LogResult"
description: "Creates a result text. The analysis automation continues the script."
---

# IVbsContextASDeinit.LogResult

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: LogResult for ContextFinalize <Analysis Automation>

Creates a result text. The analysis automation continues the script.

## Signature

```python
obj.LogResult(message)
```

## Python example

```python
def On_Finalize(oContext):
    oContext.LogResult("Number of analyzed data: " + oContext.DataLinks.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_LogResult_IVbsContextASDeinit.htm`*
