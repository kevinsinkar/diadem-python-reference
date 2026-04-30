---
title: "TdmsFileDefrag"
description: "Defragments a TDMS file in order to read it faster."
---

# TdmsFileDefrag

!!! abstract "Command &middot; `ComOff.chm`"
    Command: TdmsFileDefrag

Defragments a TDMS file in order to read it faster.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path, DIAdem uses the NAVIGATOR user path for loading or saving.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DataFileName</td>
<td>Specifies the name of a data file with the filename extension and the path.<div id="exp_DataFileName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you do not specify a path, DIAdem uses the NAVIGATOR user path for loading or saving.</td></tr></table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean variable</a> type. The return value is <span class="Monospace">True</span> if the TDMS file was successfully defragmented. Otherwise the return value is <span class="Monospace">False</span>. </td></tr>
</table>
</div>

## Python example

```python
oMyQueryForm = dd.Navigator.Display.CurrDataFinder.QueryForm
oMyQueryForm.Clear()

oMyQueryForm.Mode = dd.eAdvancedQueryForm
#--- Fill the query
oMyQueryForm.Conditions.Add(dd.eSearchFile,"dataPluginName","=","TDMS")
oMyQueryForm.Conditions.Add(dd.eSearchFile,"ni_df_defragmentation_needed","=","1")
oMyQueryForm.Conditions.Add(dd.eSearchFile,"ni_df_defragmentation_done","=","0")
oMyQueryForm.Conditions.Add(dd.eSearchFile,"ni_df_indexfile_invalid","=","1")
oMyQueryForm.Conditions.Logic = "C1 and ((C2 and C3) or C4)"
oMyQueryForm.Search()

oMyResults = dd.Navigator.Display.CurrDataFinder.ResultsList.Elements

if (oMyResults.Count == 0) :
    dd.MsgBoxDisp ("No files found for defragmentation",None ,None ,None ,5)
else:
    dd.MsgBoxDisp ("Number of files for defragmentation: " + oMyResults.Count,None ,None ,None ,3)

    for oMyElementT in oMyResults:
        dd.MsgBoxDisp ("TdmsFileDefrag of " + oMyElementT.Properties("fullpath").Value,"MB_NOBUTTON", "MsgTypeNote",None ,None ,True)
        dd.TdmsFileDefrag (oMyElementT.Properties("fullpath").Value )
        dd.MsgBoxCancel()
```

---

*Source: `ComOff/TdmsFileDefrag.htm`*
