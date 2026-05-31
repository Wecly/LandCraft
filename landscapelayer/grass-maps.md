# 🌿 Grass Maps

![](<../images/image24.jpg>)

Controls per-layer grass density maps used by Unreal's Landscape Grass system. Each density slot drives a separate grass type. Noise masking enables natural variation in grass placement.

---

### Setup

| Parameter | Description |
|-----------|-------------|
| **Add GrassMaps** | Enables grass map output for this layer — must be active for any grass to be placed. |
| **Grass Noise Mask** | Enables noise-based masking of the grass density maps for natural breakup. |

---

![](<../images/image6.jpg>)

### Noise Mask

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Grass Noise Channel** | Texture channel driving the grass noise mask. | Green |
| **Grass Noise Amount** | Strength of the noise mask. | `0.0` |
| **Grass Noise Contrast** | Contrast of the noise mask. | `1.0` |
| **Grass Noise Index** | Selects which noise texture index is used (1–6). | `1.0` |

---

### Density Slots

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Grass1 Density** | Density value for grass slot 1. | `0.0` |
| **Grass2 Density** | Density value for grass slot 2. | `0.0` |
| **Grass3 Density** | Density value for grass slot 3. | `0.0` |
| **Grass4 Density** | Density value for grass slot 4. | `0.0` |
| **Grass5 Density** | Density value for grass slot 5. | `0.0` |
| **Grass6 Density** | Density value for grass slot 6. | `0.0` |
