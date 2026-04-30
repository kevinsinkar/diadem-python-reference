---
title: "IVbsDataLinksCollection.Count"
description: "Returns the number of elements in a search. If you execute a comparative evaluation, the DataLinks <Analysis Automation> collection contains all elements of the"
---

# IVbsDataLinksCollection.Count

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: Count for DataLinks <Analysis Automation>

Returns the number of elements in a search. If you execute a comparative evaluation, the DataLinks <Analysis Automation> collection contains all elements of the search. If you execute a parallel evaluation, the DataLinks <Analysis Automation> collection always contains exactly one element.

## Signature

```python
obj.Count
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

*Source: `TDMcontext/properties/TDMContext_property_Count_IVbsDataLinksCollection.htm`*
