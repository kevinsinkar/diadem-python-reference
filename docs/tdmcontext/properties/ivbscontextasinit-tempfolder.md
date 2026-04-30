---
title: "IVbsContextASInit.TempFolder"
description: "Returns the path to the current temporary folder. The temporary folder is different for each procedure call in the analysis automation and is deleted after the "
---

# IVbsContextASInit.TempFolder

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: TempFolder for ContextInitialize <Analysis Automation>

Returns the path to the current temporary folder. The temporary folder is different for each procedure call in the analysis automation and is deleted after the procedure has been executed.

## Signature

```python
obj.TempFolder
```

## Python example

```python
def On_Initialize(oContext):
    ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
    oContext.LogResult("Results path for init: " + ResultsPath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_TempFolder_IVbsContextASInit.htm`*
