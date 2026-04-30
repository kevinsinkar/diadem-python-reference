---
title: "AnalysisProcedure.On_Run_AnalysisProcedure"
description: "Use this event to add user-defined program code with which the analysis automation procedure analyzes the elements from the search. This event is called several"
---

# AnalysisProcedure.On_Run_AnalysisProcedure

!!! abstract "Event &middot; `TDMcontext.chm`"
    Event: On_Run_AnalysisProcedure

Use this event to add user-defined program code with which the analysis automation procedure analyzes the elements from the search. This event is called several times if you select the evaluation mode Each retrieved element is processed individually (in parallel) on the Analysis Script tab in the analysis automation procedure. If you select the evaluation mode All retrieved elements are processed together (comparative evaluation) , the event is called only once.

## Signature

```python
dd.On_Run_AnalysisProcedure(oContext)
```

---

*Source: `TDMcontext/procedures/On_Run_AnalysisProcedure.htm`*
