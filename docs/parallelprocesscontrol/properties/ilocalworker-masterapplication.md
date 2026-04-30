---
title: "ILocalWorker.MasterApplication"
description: "Specifies which master application started the Worker object. Use the MasterApplication property to request, for example, the value of a global variable such as"
---

# ILocalWorker.MasterApplication

!!! abstract "Property &middot; `ParallelProcessControl.chm`"
    Property: MasterApplication for LocalWorker

Specifies which master application started the Worker object. Use the MasterApplication property to request, for example, the value of a global variable such as R1 in the master. Do not use this property, for example, to start a script in the master because the worker waits until the master application answers.

## Signature

```python
return_value = obj.MasterApplication
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="../../objects/ilocalworker/">Objects Overview</a></p>
</div>
</div>

---

*Source: `ParallelProcessControl/properties/ParallelProcessControl_property_MasterApplication_ILocalWorker.htm`*
