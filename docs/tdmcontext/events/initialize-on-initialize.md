---
title: "Initialize.On_Initialize"
description: "Use this event to initialize parallel processing. This event is only called if you select the evaluation mode Each retrieved element is processed individually ("
---

# Initialize.On_Initialize

!!! abstract "Event &middot; `TDMcontext.chm`"
    Event: On_Initialize

Use this event to initialize parallel processing. This event is only called if you select the evaluation mode Each retrieved element is processed individually (in parallel) on the Analysis Script tab in the analysis automation procedure. The event is called once before the data is processed.

## Signature

```python
dd.On_Initialize(oContext)
```

---

*Source: `TDMcontext/procedures/On_Initialize.htm`*
