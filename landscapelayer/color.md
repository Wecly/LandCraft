# 🎨 Color

![](<../images/image34.jpg>)

Controls albedo color adjustments — brightness, tint, contrast, desaturation — applied on top of the texture. Albedo Mask support allows isolating color changes to specific texture regions.

---

### Base Color

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Brightness** | Overall brightness multiplier for the albedo. | `1.0` |
| **Tint Color** | Color tint applied multiplicatively over the albedo. | White (no tint) |
| **Contrast** | Adjusts albedo contrast. Positive values increase contrast. | `0.0` |
| **Desaturation** | Desaturates the albedo. `0.0` = full color, `1.0` = fully gray. | `0.0` |

---

![](<../images/image10.jpg>)

### ♦ use Albedo Mask

Enables a mask that restricts color adjustments to specific texture regions.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Displacement - use Roughness Mask** | Uses the Roughness channel as the mask source. | — |
| **AlbedoMask Amount** | Blend amount of the albedo mask. | `0.0` |
| **AlbedoMask Contrast** | Contrast of the albedo mask. | `1.0` |
| **Albedo Mask Desaturation** | Desaturation within the masked region. | `0.0` |
| **Albedo Mask Brightness** | Brightness within the masked region. | `1.0` |
| **Albedo Mask Tint** | Color tint within the masked region. | — |
