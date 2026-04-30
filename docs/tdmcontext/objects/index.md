---
title: "Objects (TDM Context)"
---

# Objects

15 objects from `TDMcontext.chm`.

| Name | Summary |
| --- | --- |
| [`IVbsArgument`](ivbsargument.md) | The Argument <SystemLink> object provides an argument in Data Preparation or Analysis Automation. |
| [`IVbsContextAS`](ivbscontextas.md) | The ContextRun <Analysis Automation> object provides information on the analysis automation event On_Run_AnalysisProcedure . The On_Run_AnalysisProcedure event is called several times if you execute a parallel analysis, otherwise it is called only once. |
| [`IVbsContextASDeinit`](ivbscontextasdeinit.md) | The ContextFinalize <Analysis Automation> object provides information on the analysis automation event On_Finalize . The On_Finalize event is only called if you execute a parallel analysis. |
| [`IVbsContextASInit`](ivbscontextasinit.md) | The ContextInitialize <Analysis Automation> object provides information on the analysis automation event On_Initialize . The On_Initialize event is only called if you execute a parallel analysis. |
| [`IVbsContextVnV`](ivbscontextvnv.md) | The ContextVnV <Data Preprocessor> object provides information on the data preparation event On_ValidationAndVerification . |
| [`IVbsCurrDataProvider`](ivbscurrdataprovider.md) | The CurrDataProvider <Analysis Automation> object provides the properties of the current data store or DataFinder. Define the data source to use in the associated task in the analysis automation. Use the CurrDataProvider <Analysis Automation> object to open a connection to the current DataFinder or data store with the ConnectDataFinderByParameter for Navigator and ConnectDataStoreByParameter for Navigator methods in order to execute additional searches there. |
| [`IVbsFileService`](ivbsfileservice.md) | The FileService <SystemLink> object allows you to upload files to the SystemLink file service. You can also find the uploaded files in the results of current and completed analysis automation tasks. You can download them from there or open them in the SystemLink File Viewer. |
| [`IVbsJob`](ivbsjob.md) | The Procedure <Analysis Automation> object provides information on the current procedure being executed. |
| [`IVbsProcedureInfo`](ivbsprocedureinfo.md) | The ProcedureInfo <Analysis Automation> object provides information on the task being executed. |
| [`IVbsStatus`](ivbsstatus.md) | The Status <Analysis Automation> object provides the information on whether the events On_Initialize and On_Run_AnalysisProcedure were successful. The event On_Finalize is always called, even if the events On_Initialize and On_Run_AnalysisProcedure were not successful. |
| [`IVbsSubtaskInfo`](ivbssubtaskinfo.md) | The SubTaskInfo <Analysis Automation> object provides information on the subtask being executed. |
| [`IVbsTags`](ivbstags.md) | The Tags <SystemLink> object creates and modifies SystemLink tags and returns the tag values. Tags correspond to variables that are valid throughout the SystemLink environment and that you can access via a unique identifier. |
| [`IVbsTaskExecution`](ivbstaskexecution.md) | The TaskExecution <Analysis Automation> object provides information on the task being executed. The TaskInfo object contains information on the executable task. The ProcedureInfo object contains information on the analysis automation procedure of a task. |
| [`IVbsTaskInfo`](ivbstaskinfo.md) | The TaskInfo <Analysis Automation> object provides information about a task from the list of executable tasks. The TaskExecution object contains information on the executed task. The ProcedureInfo object contains information on the analysis automation procedure of a task. |
| [`IVbsUserInfo`](ivbsuserinfo.md) | The UserInfo <Analysis Automation> object provides information about the user who is searching for data in the current task. |
