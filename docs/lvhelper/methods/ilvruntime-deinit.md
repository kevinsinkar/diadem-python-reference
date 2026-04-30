---
title: "ILVRuntime.DeInit"
description: "Unloads the LabVIEW Run Time Library and disconnects LabVIEW."
---

# ILVRuntime.DeInit

!!! abstract "Method &middot; `LVHelper.chm`"
    Method: DeInit for LVRuntime

Unloads the LabVIEW Run Time Library and disconnects LabVIEW.

## Signature

```python
obj.DeInit
```

## Python example

```python
# Initialize the LVRuntime
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)

# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test")

# Call the VI
objVI.Run(True)
# Clean upSet VIT = Nothing
dd.LVRuntime.DeInit()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/methods/LVHelper_method_DeInit_ILVRuntime.htm`*
