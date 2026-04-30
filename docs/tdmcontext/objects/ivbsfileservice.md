---
title: "IVbsFileService"
description: "The FileService <SystemLink> object allows you to upload files to the SystemLink file service. You can also find the uploaded files in the results of current an"
---

# IVbsFileService

!!! abstract "Object &middot; `TDMcontext.chm`"
    Object: FileService <SystemLink>

The FileService <SystemLink> object allows you to upload files to the SystemLink file service. You can also find the uploaded files in the results of current and completed analysis automation tasks. You can download them from there or open them in the SystemLink File Viewer.

## Python example

```python
def On_Finalize(oContext):
    ResultsPath = oContext.Procedure.Arguments.Item("ResultsPath").Value
    dd.Report.ActiveSheet.ExportToPDF(ResultsPath + "Result.pdf",False)
    sProperty = "{\"Resultpath\": \"" + ResultsPath.replace("\\", "\\\\") + "\"}"
    oContext.FileService.UploadResultFile(ResultsPath + "\\Result.pdf", sProperty, "" ,False)
```

## Members

<div markdown="1">
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivbsfileservice-uploadresultfile/">UploadResultFile</a> | <a href="../../methods/ivbsfileservice-uploadresultfiletoworkspace/">UploadResultFileToWorkspace</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ivbscontextasdeinit/">ContextFinalize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasdeinit-fileservice/">FileService</a> | <a href="../ivbscontextasinit/">ContextInitialize &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextasinit-fileservice/">FileService</a> | <a href="../ivbscontextas/">ContextRun &lt;Analysis Automation&gt;</a>.<a href="../../properties/ivbscontextas-fileservice/">FileService</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `TDMcontext/objects/TDMContext_Objects_IVbsFileService.htm`*
