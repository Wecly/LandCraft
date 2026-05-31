# 🌿 Grass Maps

![](<../images/image19.jpg>)

Controls the landscape grass density maps used to drive Unreal's foliage placement system. Supports anchor mask integration and noise-based breakup for natural variation in grass distribution.

---

### Setup

| Parameter | Description |
|-----------|-------------|
| **Only Grass Layer** | Restricts this blender to only output grass map data — skips all surface material blending. |
| **use AnchorMask** | Uses the saved Anchor Mask to gate grass placement — grass only appears where the Anchor Mask is active. |
| **use Grass Noise Breakup** | Applies noise-based breakup to the grass density output for natural variation. |

---

### Density Output

| Parameter | Description | Default |
|-----------|-------------|---------|
| **GrassMap Amount** | Global multiplier on the grass map output. | `0.0` |
| **GrassMap Contrast** | Contrast of the grass map mask. | `1.0` |

---

### Noise Breakup

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Grass Noise Channel** | Texture channel used for grass noise breakup. | Green |
| **Grass Noise Amount** | Amplitude of the grass noise breakup. | `0.0` |
| **Grass Noise Contrast** | Contrast of the grass noise mask. | `1.0` |
