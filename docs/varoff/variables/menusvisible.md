---
title: "MenusVisible"
description: "Valid names: MenusVisible, ApplicationMenuVisible"
---

# MenusVisible

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: MenusVisible

Valid names: MenusVisible, ApplicationMenuVisible

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Use the <a href="#" data-unresolved="1">BarManager object</a> to change and to manage buttons and bars, and also menus if they are not context menus. If you press &lt;Ctrl-Shift&gt; and idle the cursor on a bar element, DIAdem displays a tooltip with the name of the bar, the name of the bar element, and the name of the base object or base type. DIAdem also copies this information, separated by a space, to the clipboard.<br attr="ext"/>After you have changed the DIAdem interface with a script, a prompt asks you whether you want to save the changed bar definition. You can change this behavior with the <a href="../../../tobarmanagerint/properties/tobarmanageruiint-desktopmodified/">DesktopModified for BarManager </a> property.<br attr="ext"/>The following example uses the BarManager object to hide all the menu bars in all DIAdem panels but nevertheless defines the bar definition as unchanged.<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue">
<p class="body"><a href="#">Copy script</a></p></div>
<div class="codeblue"><pre><donottranslate><span class="HlVBSKeyword">Dim</span> bDesktopModified
bDesktopModified = <span class="Hldiademobject">BarManager.DesktopModified</span>
<span class="Hldiademobject">BarManager.Bars</span>(<span class="HlString">"NAVMenuMain"</span>).Visible = <span class="HlVBSKeyword">false</span>
<span class="Hldiademobject">BarManager.Bars</span>(<span class="HlString">"VIEWMenuMain"</span>).Visible = <span class="HlVBSKeyword">false</span>
<span class="Hldiademobject">BarManager.Bars</span>(<span class="HlString">"ANAMenuMain"</span>).Visible = <span class="HlVBSKeyword">false</span>
<span class="Hldiademobject">BarManager.Bars</span>(<span class="HlString">"REPMenuMain"</span>).Visible = <span class="HlVBSKeyword">false</span>
<span class="Hldiademobject">BarManager.Bars</span>(<span class="HlString">"DACMenuMain"</span>).Visible = <span class="HlVBSKeyword">false</span>
<span class="Hldiademobject">BarManager.Bars</span>(<span class="HlString">"VISMenuMain"</span>).Visible = <span class="HlVBSKeyword">false</span>
<span class="Hldiademobject">BarManager.Bars</span>(<span class="HlString">"SCRMenuMain"</span>).Visible = <span class="HlVBSKeyword">false</span>
<span class="Hldiademobject">BarManager.DesktopModified</span> = bDesktopModified</donottranslate></pre></div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>bDesktopModified = dd.BarManager.DesktopModified 
dd.BarManager.Bars(<span class="HlString">"NAVMenuMain"</span>).Visible = <span class="HlVBSKeyword">False</span> 
dd.BarManager.Bars(<span class="HlString">"VIEWMenuMain"</span>).Visible = <span class="HlVBSKeyword">False</span> 
dd.BarManager.Bars(<span class="HlString">"ANAMenuMain"</span>).Visible = <span class="HlVBSKeyword">False</span> 
dd.BarManager.Bars(<span class="HlString">"REPMenuMain"</span>).Visible = <span class="HlVBSKeyword">False</span> 
dd.BarManager.Bars(<span class="HlString">"DACMenuMain"</span>).Visible = <span class="HlVBSKeyword">False</span> 
dd.BarManager.Bars(<span class="HlString">"VISMenuMain"</span>).Visible = <span class="HlVBSKeyword">False</span> 
dd.BarManager.Bars(<span class="HlString">"SCRMenuMain"</span>).Visible = <span class="HlVBSKeyword">False</span> 
dd.BarManager.DesktopModified = bDesktopModified </donottranslate></pre></div></td></tr></table>
</div>

## Python example

```python
bDesktopModified = dd.BarManager.DesktopModified
dd.BarManager.Bars("NAVMenuMain").Visible = False
dd.BarManager.Bars("VIEWMenuMain").Visible = False
dd.BarManager.Bars("ANAMenuMain").Visible = False
dd.BarManager.Bars("REPMenuMain").Visible = False
dd.BarManager.Bars("DACMenuMain").Visible = False
dd.BarManager.Bars("VISMenuMain").Visible = False
dd.BarManager.Bars("SCRMenuMain").Visible = False
dd.BarManager.DesktopModified = bDesktopModified
```

---

*Source: `VarOff/MenusVisible.htm`*
