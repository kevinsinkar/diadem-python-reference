---
title: "AutoActPath"
description: "Specifies the path of the script file currently running. Use the CurrentScriptPath variable instead of this variable."
---

# AutoActPath

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: AutoActPath

Specifies the path of the script file currently running. Use the CurrentScriptPath variable instead of this variable.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The variable only receives a value when the script is running. When the script has finished, the variable receives an empty string. The command <a href="../../../comoff/commands/scriptstart/">ScriptStart</a> sets the variable <span class="Monospace">AutoActPath</span>. In user commands or in the preview of a user dialog box does not DIAdem set the <span class="Monospace">AutoActPath</span> variable.</td></tr></table>
</div>

---

*Source: `VarOff/AutoActPath.htm`*
