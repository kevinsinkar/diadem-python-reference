---
title: "IVbsContextVnV.MarkDataAsValid"
description: "Marks the data to be processed as valid."
---

# IVbsContextVnV.MarkDataAsValid

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: MarkDataAsValid for ContextVnV <Data Preprocessor>

Marks the data to be processed as valid.

## Signature

```python
obj.MarkDataAsValid
```

## Python example

```python
def On_ValidationAndVerification(oContext):
    if (dd.Data.Root.ActiveChannelGroup.Channels(1).Name == "Time") :
        oContext.MarkDataAsValid()
    else:
        oContext.MarkDataAsInvalid("Time channel does not exist")
    if oContext.IsDataValid :
        pass # do something
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_MarkDataAsValid_IVbsContextVnV.htm`*
