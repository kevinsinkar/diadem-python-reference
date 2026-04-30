---
title: "IVIRuntime.Run"
description: "Synchronous start of a LabVIEW VI which means DIAdem waits until the VI stops before DIAdem executes a script."
---

# IVIRuntime.Run

!!! abstract "Method &middot; `LVHelper.chm`"
    Method: Run for VIRuntime

Synchronous start of a LabVIEW VI which means DIAdem waits until the VI stops before DIAdem executes a script.

## Signature

```python
bRun = Object.Run(Visible)
```

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
objVI.run(True)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/methods/LVHelper_method_Run_IVIRuntime.htm`*
