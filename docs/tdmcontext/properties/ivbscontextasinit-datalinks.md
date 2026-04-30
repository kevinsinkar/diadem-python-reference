---
title: "IVbsContextASInit.DataLinks"
description: "Returns the DataLinks <Analysis Automation> collection. If you execute a comparative evaluation, the DataLinks <Analysis Automation> collection contains all ele"
---

# IVbsContextASInit.DataLinks

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: DataLinks for ContextInitialize <Analysis Automation>

Returns the DataLinks <Analysis Automation> collection. If you execute a comparative evaluation, the DataLinks <Analysis Automation> collection contains all elements of the search. Otherwise, DIAdem runs the search simultaneously, and the DataLinks <Analysis Automation> collection always contains exactly one element.

## Signature

```python
return_value = obj.DataLinks
```

## Python example

```python
def On_Initialize(oContext):
    oContext.LogResult("Number of data sources to be analyzed: " + oContext.DataLinks.Count)
# Enter your analysis commands
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_DataLinks_IVbsContextASInit.htm`*
