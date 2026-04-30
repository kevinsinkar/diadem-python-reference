---
title: "ApplicationPreviewFeatureIndexGet"
description: "Specifies the index of a preview feature."
---

# ApplicationPreviewFeatureIndexGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ApplicationPreviewFeatureIndexGet

Specifies the index of a preview feature.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ApplicationPreviewFeature</td>
<td>Specifies the ID of the preview feature.<div id="exp_ApplicationPreviewFeature">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer</a></td></tr>
<tr>
<td>1 &lt;= ApplicationPreviewFeature &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Integer</a> type. Contains the index of the preview feature.</td></tr>
</table>
</div>

## Python example

```python
FeatureID = 1145367
dd.ApplicationEnablePreviewFeature = True
print(dd.ApplicationPreviewFeatureIndexGet(FeatureID))
```

---

*Source: `ComOff/ApplicationPreviewFeatureIndexGet.htm`*
