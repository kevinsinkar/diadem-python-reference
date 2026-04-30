---
title: "ImageFileToIconFile"
description: "Converts a graphic file into an ICO file."
---

# ImageFileToIconFile

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ImageFileToIconFile

Converts a graphic file into an ICO file.

## Signature

```python
dd.ImageFileToIconFile(ImageFile, IconTargetPath, ImageTransparentColor)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ImageFile</td>
<td>Specifies the name and the path of the graphics file. Supported file types: .bmp, .jpg, .tif, .wmf, .emf, .pcx, .png, and .gif.<div id="exp_ImageFile">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">IconTargetPath</td>
<td>Specifies the absolute path where DIAdem saves the generated ICO file. If the path entry is blank, DIAdem saves the ICO file in the source path.<div id="exp_IconTargetPath">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ImageTransparentColor</td>
<td>Specifies the <a href="#" data-unresolved="1">RGB value</a> of the transparent color. If the value is -1, DIAdem does not use transparent color.<div id="exp_ImageTransparentColor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>-1 &lt;= ImageTransparentColor &lt;= 16777215</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ImageFileToIconFile.htm`*
