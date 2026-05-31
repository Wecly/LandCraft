# 🎨 Paint Mask

![](<../images/image3.jpg>)

Drives layer blending via Unreal's landscape paint data. Supports additive layer painting, erase painting, and can be repurposed as a grass remover channel for precise foliage control.

---

| Parameter | Description | Default |
|-----------|-------------|---------|
| **LayerPaint** | Enables landscape paint layer input — uses painted weightmap data to drive the blend mask. | — |
| **Landscape Layer Amount** | Multiplier applied to the painted layer weight before blending. | `0.0` |
| **Landscape Layer Contrast** | Contrast applied to the painted weight mask. | `1.0` |
| **Landscape Layer Sample** | RGBA channel selection for the landscape layer sample. | R=1, G=0, B=0, A=0 |
| **LayerErease** | Enables erase mode — painted areas subtract from the blend instead of adding. | — |
| **Erease Amount** | Strength of the erase effect. | `0.0` |
| **Paint as GrassRemover** | Repurposes the paint mask as a grass removal channel — painted areas suppress grass placement. | — |
