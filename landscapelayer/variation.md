# 🎲 Variation

![](<../images/image33.jpg>)

Adds procedural noise-based surface variation — breaks up material uniformity with color, roughness, displacement, and normal noise overlays.

---

### ♦ use Noise Overlay

Enables a procedural noise overlay that adds variation across the surface.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Noise Texture - use Cloud Noise** | Uses cloud noise instead of a custom texture. | — |
| **Noise Texture** | Texture driving the variation pattern. | `T_RGB_Mask` |
| **Noise Scale** | UV tiling scale of the variation noise. | `1.0` |
| **Noise Offset X** | UV offset on X axis. | `0.0` |
| **Noise Offset Y** | UV offset on Y axis. | `0.0` |

---

### ♦ use Noise Color

Applies color variation using the noise texture.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Noise Color** | Color applied as the variation tint. | — |
| **Noise Color Channel** | Texture channel driving color variation. | Red |
| **Noise Color Amount** | Blend amount of the noise color. | `0.0` |
| **Noise Color Contrast** | Contrast of the noise color mask. | `1.0` |

---

### ♦ use Noise Roughness

Applies roughness variation using the noise texture.

### ♦ use Noise Displacement

Applies displacement variation using the noise texture — adds micro-height variation.

### ♦ use Noise Normal

Adds normal variation using the noise texture — creates subtle surface perturbation without extra geometry.
