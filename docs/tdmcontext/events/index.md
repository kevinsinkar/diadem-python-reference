---
title: "Events (TDM Context)"
---

# Events

4 events from `TDMcontext.chm`.

| Name | Summary |
| --- | --- |
| [`AnalysisProcedure.On_Run_AnalysisProcedure`](analysisprocedure-on-run-analysisprocedure.md) | Use this event to add user-defined program code with which the analysis automation procedure analyzes the elements from the search. This event is called several times if you select the evaluation mode Each retrieved element is processed individually (in parallel) on the Analysis Script tab in the analysis automation procedure. If you select the evaluation mode All retrieved elements are processed together (comparative evaluation) , the event is called only once. |
| [`Finalize.On_Finalize`](finalize-on-finalize.md) | Use this event to finalize parallel processing. This event is only called if you select the evaluation mode Each retrieved element is processed individually (in parallel) on the Analysis Script tab in the analysis automation procedure. The event is called once after the data is processed. |
| [`Initialize.On_Initialize`](initialize-on-initialize.md) | Use this event to initialize parallel processing. This event is only called if you select the evaluation mode Each retrieved element is processed individually (in parallel) on the Analysis Script tab in the analysis automation procedure. The event is called once before the data is processed. |
| [`ValidationAndVerification.On_ValidationAndVerification`](validationandverification-on-validationandverification.md) | Use this event to insert your own program code, which the data preparation uses to check the loaded data. |
