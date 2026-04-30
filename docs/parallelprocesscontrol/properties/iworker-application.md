---
title: "IWorker.Application"
description: "Specifies in which application the Worker object runs. Use the Application property to, for example, request the value of a global variable, such as R1, in orde"
---

# IWorker.Application

!!! abstract "Property &middot; `ParallelProcessControl.chm`"
    Property: Application for Worker

Specifies in which application the Worker object runs. Use the Application property to, for example, request the value of a global variable, such as R1, in order to check the progress in the worker. The worker does not answer until it is no longer busy. In this time the master does not execute any other commands. Therefore you should only use this property in exceptional cases.

## Signature

```python
return_value = obj.Application
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Parallel File Analysis</a> | <a href="#" data-unresolved="1">Vibration Data Analysis with Parallel Processing</a></p>
</div>
</div>

---

*Source: `ParallelProcessControl/properties/ParallelProcessControl_property_Application_IWorker.htm`*
