---
title: "PeakDetectWidth"
description: "Specifies the number of successive points, which DIAdem uses for the adaptation with the least squares method. The value must be greater than or equal to three."
---

# PeakDetectWidth

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: PeakDetectWidth

Specifies the number of successive points, which DIAdem uses for the adaptation with the least squares method. The value must be greater than or equal to three. The value should be at least half the width of the peaks or valleys and below that if the signals are noiseless. If the widths are large, you can decrease the apparent peak amplitudes and move the apparent position. If the data is noisy, this change is insignificant because the noise hides the actual peak. Select the smallest possible width, which is still large enough to preclude incorrect peak values created by noise.

---

*Source: `VarOff/PeakDetectWidth.htm`*
