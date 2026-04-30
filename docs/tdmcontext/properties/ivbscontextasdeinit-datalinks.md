---
title: "IVbsContextASDeinit.DataLinks"
description: "Returns the DataLinks <Analysis Automation> collection. If you execute a comparative evaluation, the DataLinks <Analysis Automation> collection contains all ele"
---

# IVbsContextASDeinit.DataLinks

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: DataLinks for ContextFinalize <Analysis Automation>

Returns the DataLinks <Analysis Automation> collection. If you execute a comparative evaluation, the DataLinks <Analysis Automation> collection contains all elements of the search. Otherwise, DIAdem runs the search simultaneously, and the DataLinks <Analysis Automation> collection always contains exactly one element.

## Signature

```python
return_value = obj.DataLinks
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    oContext.LogResult("Number of analyzed data sources: " + oContext.DataLinks.Count)
# Enter your analysis commands
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_DataLinks_IVbsContextASDeinit.htm`*
