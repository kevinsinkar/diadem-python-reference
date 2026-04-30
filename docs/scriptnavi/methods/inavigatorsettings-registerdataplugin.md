---
title: "INavigatorSettings.RegisterDataPlugin"
description: "Registers a DataPlugin in DIAdem."
---

# INavigatorSettings.RegisterDataPlugin

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: RegisterDataPlugin for Settings <Navigator>

Registers a DataPlugin in DIAdem.

## Signature

```python
bRegisterDataPlugin = Object.RegisterDataPlugin(UriFileName, SilentMode)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  You can double-click the associated uri file to register a DataPlugin.</td></tr></table>
</div>

## Python example

```python
dd.Navigator.Settings.RegisterDataPlugin("c:\\ProgramData\\National Instruments\\Shared\\USI\\Plugins\\DataPlugins\\NMEA_GPS\\NMEA_GPS.uri", False)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_RegisterDataPlugin_INavigatorSettings.htm`*
