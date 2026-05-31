# ⚙️ Blend

![](<../images/image5.png>)

Controls how layers are blended together — which material channels participate in the blend, how weighting works, and per-channel blend behavior for BaseColor, Roughness, Normal, Displacement, WPO, and Specular.

---

### Debug Tools

| Parameter | Description |
|-----------|-------------|
| **🔎 Debug** | Enables debug visualization of the blend result. Useful for diagnosing mask and channel issues. |
| **🔎 Debug Base Mask** | Visualizes the Base Mask driving the blend in the viewport. |
| **🔎 Debug Grass Map** | Visualizes the Grass Map output in the viewport. |
| **🔎 Debug Paint Mask** | Visualizes the Paint Mask in the viewport. |

---

![](<../images/image20.jpg>)

### 🔷 Material - use Attribute Blend

Switches to per-channel attribute blend mode — enables independent control over which material channels participate in the blend.

| Parameter | Description |
|-----------|-------------|
| **use Attribute Weights** | Enables per-channel weight control for the attribute blend. |
| **use Material from Bottom Layer** | Forces material attributes to be read from the bottom layer instead of blending. |

---

### 🔶 use BaseColor

Controls BaseColor blending between layers.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **use BaseColor from Bottom Layer** | Uses the bottom layer's BaseColor as the blend result. | — |
| **Desaturation** | Desaturates the blended BaseColor result. | `0.0` |
| **Tint Color** | Color tint applied to the blended BaseColor. | White |
| **BaseColor Weight** | Weight of the top layer BaseColor in the blend. | `1.0` |

---

### 🔶 use Roughness

Controls Roughness blending between layers.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **use Roughness from Bottom Layer** | Forces Roughness from the bottom layer. | — |
| **Roughness Amount** | Additive offset on the blended Roughness. | `0.0` |
| **Roughness Weight** | Weight of the top layer Roughness in the blend. | `1.0` |

---

### 🔶 use Normal

Controls Normal blending between layers.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **use Normal Blend** | Enables normal blending between the two layers. | — |
| **use Normal from Bottom Layer** | Forces Normal from the bottom layer. | — |
| **Normal Intensity** | Blend intensity for the normal. | `1.0` |
| **Normal Weight** | Weight of the top layer Normal in the blend. | `1.0` |

---

### 🔶 use Displacement

Controls Displacement blending between layers.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **use Displacement from Bottom Layer** | Forces Displacement from the bottom layer. | — |
| **Displacement Amount** | Additive displacement offset. | `0.0` |
| **Displacement Weight** | Weight of top layer Displacement in blend. | `1.0` |
| **use WPO from Bottom Layer** | Forces WPO from the bottom layer. | — |

---

### 🔶 use WPO

Controls World Position Offset blending.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **WPO Amount** | Additive WPO offset. | `0.0` |
| **WPO Weight** | Weight of top layer WPO in blend. | `1.0` |
| **Specular Weight** | Weight of top layer Specular in blend. | `1.0` |
