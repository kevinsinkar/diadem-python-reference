---
title: "IVbsContextVnV"
description: "The ContextVnV <Data Preprocessor> object provides information on the data preparation event On_ValidationAndVerification ."
---

# IVbsContextVnV

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: ContextVnV <Data Preprocessor>

The ContextVnV <Data Preprocessor> object provides information on the data preparation event On_ValidationAndVerification .

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivbscontextvnv-arguments/">Arguments</a> | <a href="../../properties/ivbscontextvnv-isdatavalid/">IsDataValid</a> | <a href="../../properties/ivbscontextvnv-tags/">Tags</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivbscontextvnv-logerror/">LogError</a> | <a href="../../methods/ivbscontextvnv-markdataasinvalid/">MarkDataAsInvalid</a> | <a href="../../methods/ivbscontextvnv-markdataasvalid/">MarkDataAsValid</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsContextVnV.htm`*
