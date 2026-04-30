---
title: "IVbsContextAS.Procedure"
description: "Returns an object that provides information on the procedure currently being executed."
---

# IVbsContextAS.Procedure

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: Procedure for ContextRun <Analysis Automation>

Returns an object that provides information on the procedure currently being executed.

## Signature

```python
return_value = obj.Procedure
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
    oContext.LogResult("Results path: " + ResultsPath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_Procedure_IVbsContextAS.htm`*
