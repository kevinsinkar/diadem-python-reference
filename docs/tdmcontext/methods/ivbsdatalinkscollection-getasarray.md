---
title: "IVbsDataLinksCollection.GetAsArray"
description: "Returns an element of the DataLinks <Analysis Automation> collection as a type-safe array. You cannot access this array from VBS scripts. However, you can excha"
---

# IVbsDataLinksCollection.GetAsArray

!!! abstract "Method &middot; `TDMcontext.chm`"
    Method: GetAsArray for DataLinks <Analysis Automation>

Returns an element of the DataLinks <Analysis Automation> collection as a type-safe array. You cannot access this array from VBS scripts. However, you can exchange the data with other applications that expect type-safe arrays. You can use this array in the LoadData for Navigator command in order to load the elements from the search simultaneously. This method may use a lot of memory because analysis automation loads all retrieved data simultaneously. However, analysis automation does not need to load this data individually through the network, which may improve performance. Use the Item for DataLinks method to access the data one by one.

## Signature

```python
obj.GetAsArray
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    dd.Navigator.LoadData(oContext.DataLinks.GetAsArray())
# Enter your analysis commands
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/methods/TDMContext_method_GetAsArray_IVbsDataLinksCollection.htm`*
