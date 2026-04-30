---
title: "ApplicationPreviewFeatureTitle"
description: "Specifies the title of a preview feature."
---

# ApplicationPreviewFeatureTitle

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ApplicationPreviewFeatureTitle

Specifies the title of a preview feature.

## Python example

```python
dd.ApplicationEnablePreviewFeature = True
for I in range( 1, dd.ApplicationPreviewFeatureCount+1):
    print("ID " , dd.ApplicationPreviewFeatureID(I) , "\r\n" , "Title: " , dd.ApplicationPreviewFeatureTitle(I) , "\r\n" , "Enabled: " , dd.ApplicationPreviewFeatureEnabled(I) )
```

---

*Source: `VarOff/ApplicationPreviewFeatureTitle.htm`*
