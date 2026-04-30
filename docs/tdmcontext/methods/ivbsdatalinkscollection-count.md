---
title: "IVbsDataLinksCollection.Count"
description: "Returns the number of elements of the DataLinks <Analysis Automation> collection. If you execute a comparative evaluation, the DataLinks <Analysis Automation> c"
---

# IVbsDataLinksCollection.Count

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: Count for DataLinks <Analysis Automation>

Returns the number of elements of the DataLinks <Analysis Automation> collection. If you execute a comparative evaluation, the DataLinks <Analysis Automation> collection contains all elements of the search. Otherwise, DIAdem runs the search simultaneously, and the DataLinks <Analysis Automation> collection always contains exactly one element.

## Signature

```python
iCount = Object.Count
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

*Source: `TDMcontext/methods/TDMContext_method_Count_IVbsDataLinksCollection.htm`*
