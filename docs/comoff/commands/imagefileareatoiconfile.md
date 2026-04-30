---
title: "ImageFileAreaToIconFile"
description: "Converts a rectangular extract of a graphic file into an ICO file."
---

# ImageFileAreaToIconFile

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ImageFileAreaToIconFile

Converts a rectangular extract of a graphic file into an ICO file.

## Signature

```python
dd.ImageFileAreaToIconFile(ImageFile, IconTargetPath, ImageTransparentColor, ImageAreaX, ImageAreaY, ImageAreaWidth, ImageAreaHeight)
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
<tr><td width="150">ImageAreaX</td>
<td>Specifies the distance between the rectangular section and the left edge, in pixels.<div id="exp_ImageAreaX">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ImageAreaY</td>
<td>Specifies the distance between the rectangular section and the top edge, in pixels.<div id="exp_ImageAreaY">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ImageAreaWidth</td>
<td>Specifies the width of the rectangular extract, in pixels.<div id="exp_ImageAreaWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ImageAreaHeight</td>
<td>Specifies the height of the rectangular extract, in pixels.<div id="exp_ImageAreaHeight">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
for T in range(1, 19+1):
    dd.ImageFileAreaToIconFile(dd.ProgramDrv+"Symbols\\8 Bit\\ADAdwin.bmp", dd.ResourceDrv+"BarSource", dd.RGB(255,255,255), (T-1)*27, 0, 27, 27)
    dd.FileRename(dd.ResourceDrv+"BarSource\\ADAdwin.ico",dd.ResourceDrv+"BarSource\\ADAdwin_1_" + dd.Str(T) + ".ico")
```

---

*Source: `ComOff/ImageFileAreaToIconFile.htm`*
