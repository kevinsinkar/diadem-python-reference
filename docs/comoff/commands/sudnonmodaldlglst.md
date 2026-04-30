---
title: "SUDNonModalDlgLst"
description: "Receives the list of all non-modal user dialog boxes."
---

# SUDNonModalDlgLst

!!! abstract "Command &middot; `ComOff.chm`"
    Command: SUDNonModalDlgLst

Receives the list of all non-modal user dialog boxes.

## Signature

```python
return_value = dd.SUDNonModalDlgLst(SUDNonmodalDlgId)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SUDNonmodalDlgId</td>
<td>Specifies the number or the name of a non-modal user dialog box.<div id="exp_SUDNonmodalDlgId">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="../../../sudref/objects/tosudviewobint/">Dialog object</a> type. To create a Dialog object, you assign the returned object to an object variable.</td></tr>
</table>
</div>

## Python example

```python
for i in range( 1, dd.SudNonModalDlgCount+1):
    dd.MsgBoxDisp("Dialogname = " + dd.SudNonModalDlgLst(i).DialogCode)
```

```python
MyDlg= dd.SudNonModalDlgLst("Input")
MyDlg.Color = dd.RGB(256,256,128)
MyDlg.Show
```

```python
if None is dd.SudNonModalDlgLst("Dialog1") :
    MyDlg = dd.SudDlgCreate("Dialog1","Example")
else:
    MyDlg = dd.SudNonModalDlgLst("Dialog1")
MyDlg.Show()
```

---

*Source: `ComOff/SUDNonModalDlgLst.htm`*
