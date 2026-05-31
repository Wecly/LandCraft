# 🔍 Detail Mask

![](<../images/image31.jpg>)

Fine-tunes blend transitions using height-based and noise-based detail masking. Controls how sharply or smoothly layer boundaries are defined at close range — essential for natural-looking terrain transitions.

---

### Transition Control

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Overall Transition** | Enables the overall mask effect instead of focusing only the transition area of values between 0–1. | — |
| **Blend Transition** | Enables blend-based transition sharpening using the Transition Contrast. | — |
| **Transition Contrast** | Controls the sharpness of the blend transition. Higher values create harder edges. | `10.0` |

---

### Combined Detail Mask

| Parameter | Description |
|-----------|-------------|
| **use Combined Detail Mask** | Combines HeightLerp and Cloud Noise masks to produce a richer, more organic transition edge. |
| **HeightLerp - use Noise Texture** | Uses a noise texture to drive the HeightLerp transition instead of pure height data. |
| **Bottom - use Top Layer Height** | Uses the top layer's height data instead of the bottom layer for the HeightLerp calculation. |

---

### Height Parameters

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Height Amount** | Strength of the height-based blend contribution. | `0.0` |
| **Height Contrast** | Contrast of the height mask before blending. | `2.0` |

---

![](<../images/image9.jpg>)

### Cloud Noise

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Cloud Noise - use Texture** | Enables cloud noise, using stored texture sample data instead of sampling a new one per layer. | — |
| **Texture - use Generated Noise** | Uses UE's procedural noise generator instead of a sampled texture. | — |
| **Noise Amount** | Amplitude of the noise added to the blend edge. | `0.0` |
| **Noise Contrast** | Contrast applied to the noise mask. | `4.0` |
| **Cloud Noise Channel** | Texture channel used for cloud noise sampling. | Green |
| **Noise Channel** | Texture channel used for the main noise sampling. | Green |
| **Noise Texture** | Texture asset providing the noise data. | `T_RGB_Mask` |
| **Noise Scale** | UV tiling scale of the noise texture. | `1.0` |
| **Noise Offset X** | UV offset on the X axis. | `0.0` |
| **Noise Offset Y** | UV offset on the Y axis. | `0.0` |
