---
title: "AutoAbort"
description: "Specifies whether you can abort scripts with <Esc>."
---

# AutoAbort

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: AutoAbort

Specifies whether you can abort scripts with <Esc>.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you assign the value <span class="Monospace">FALSE</span> to the <span class="Monospace">AutoAbort</span> variable you cannot abort scripts. Because some commands monitor a termination there can be exceptions.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If a script starts a second script with <a href="../../../comoff/commands/scriptstart/">ScriptStart</a> and if you abort the accessed script with &lt;Esc&gt;, DIAdem generates an error in the accessed script. You can handle this error with the <a href="#" data-unresolved="1">On Error</a> statement. Without an error handling DIAdem aborts all scripts and displays the row where you aborted.</td></tr></table>
</div>

---

*Source: `VarOff/AutoAbort.htm`*
