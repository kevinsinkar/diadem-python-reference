---
title: "IVbsContextVnV.IsDataValid"
description: "Specifies whether the processed data is marked valid. Use the methods MarkDataAsValid and MarkDataAsInvalid to mark whether the data is valid or invalid."
---

# IVbsContextVnV.IsDataValid

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: IsDataValid for ContextVnV <Data Preprocessor>

Specifies whether the processed data is marked valid. Use the methods MarkDataAsValid and MarkDataAsInvalid to mark whether the data is valid or invalid.

## Signature

```python
obj.IsDataValid
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

*Source: `TDMcontext/properties/TDMContext_property_IsDataValid_IVbsContextVnV.htm`*
