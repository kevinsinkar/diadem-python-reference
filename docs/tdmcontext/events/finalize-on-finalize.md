---
title: "Finalize.On_Finalize"
description: "Use this event to finalize parallel processing. This event is only called if you select the evaluation mode Each retrieved element is processed individually (in"
---

# Finalize.On_Finalize

!!! abstract "Event &middot; `TDMcontext.chm`"
    Event: On_Finalize

Use this event to finalize parallel processing. This event is only called if you select the evaluation mode Each retrieved element is processed individually (in parallel) on the Analysis Script tab in the analysis automation procedure. The event is called once after the data is processed.

## Signature

```python
dd.On_Finalize(oContext)
```

---

*Source: `TDMcontext/procedures/On_Finalize.htm`*
