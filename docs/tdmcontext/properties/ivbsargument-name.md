---
title: "IVbsArgument.Name"
description: "Returns the name of an argument."
---

# IVbsArgument.Name

!!! abstract "Property &middot; `TDMcontext.chm`"
    Property: Name for Argument <SystemLink>

Returns the name of an argument.

## Signature

```python
obj.Name
```

## Python example

```python
def On_Run_AnalysisProcedure(oContext):
    for Parameter in oContext.Procedure.Arguments:
        sParamName        = Parameter.Name
        vParamValue       = Parameter.Value
        sParamType        = Parameter.Type
        sParamDescription = Parameter.Description
        oContext.LogResult(sParamDescription + "\r\n" + sParamName + ": " + vParamValue + " Type: " + sParamType)
# Enter your analysis commands
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/properties/TDMContext_property_Name_IVbsArgument.htm`*
