---
title: "INaviDataFinderBrowser"
description: "The Browser object provides the file browser of a DataFinder. You also can use the file browser to browse in files."
---

# INaviDataFinderBrowser

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: Browser <DataFinder>

The Browser object provides the file browser of a DataFinder. You also can use the file browser to browse in files.

## Python example

```python
oMyBrowser = dd.Navigator.Display.CurrDataFinder.Browser
oMyFocusedElement = oMyBrowser.FocusedElement
oMyBrowser.ReindexElement(oMyFocusedElement)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/inavidatafinderbrowser-focusedelement/">FocusedElement</a> | <a href="../../properties/inavidatafinderbrowser-isactive/">IsActive</a> | <a href="../../properties/inavidatafinderbrowser-selectedelements/">SelectedElements</a> | <a href="../../properties/inavidatafinderbrowser-onlyshowsearchareas/">OnlyShowSearchAreas</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/inavidatafinderbrowser-activate/">Activate</a> | <a href="../../methods/inavidatafinderbrowser-closeall/">CloseAll</a> | <a href="../../methods/inavidatafinderbrowser-indexfolder/">IndexFolder</a> | <a href="../../methods/inavidatafinderbrowser-iskindof/">IsKindOf</a> | <a href="../../methods/inavidatafinderbrowser-refreshall/">RefreshAll</a> | <a href="../../methods/inavidatafinderbrowser-reindexelement/">ReindexElement</a> | <a href="../../methods/inavidatafinderbrowser-updatesearcharea/">UpdateSearchArea</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idatafinderdisplay/">DataFinderDisplay</a>.<a href="../../properties/idatafinderdisplay-browser/">Browser</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_INaviDataFinderBrowser.HTM`*
