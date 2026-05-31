# 🏔️ Deform

![](<../images/image13.jpg>)

Controls mesh displacement and World Position Offset — allows the surface geometry to be physically displaced or animated in world space.

---

### Displacement

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Displacement Amount** | Strength of height-based mesh displacement. | `0.0` |
| **Displacement Contrast** | Contrast of the displacement map before application. | `1.0` |

---

![](<../images/image7.png>)

### ♦ use WPO

Enables World Position Offset — moves surface vertices in world space for organic motion or surface deformation.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **VertexNormal - use Axis Direction** | Uses the vertex normal direction for WPO displacement axis. | — |
| **WPO Strength** | Intensity of the WPO displacement. | `0.0` |
| **WPO Offset** | Base vertex offset before noise. | `0.0` |

---

![](<../images/image17.jpg>)

### ♦ WPO Noise

Adds procedural noise to the WPO to create organic surface movement such as wind or water ripples.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **WPO from CloudNoise** | Uses cloud noise as the WPO noise source. | — |
| **WPO Noise Texture** | Texture driving the WPO noise pattern. | `T_PuddleMask` |
| **WPO Noise Channel** | Texture channel used for noise. | Red |
| **WPO Noise Tiling** | UV tiling of the WPO noise texture. | `1.0` |
| **WPO Noise Amount** | Amplitude of the WPO noise. | `0.0` |
| **WPO Noise Contrast** | Contrast of the noise before displacement. | `1.0` |

---

![](<../images/image14.jpg>)

### ♦ WPO Animation

Animates the WPO noise over time for continuous surface motion.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **WPO Noise Speed** | Overall animation speed. | `1.0` |
| **WPO Noise Speed X** | Animation speed on X axis. | `1.0` |
| **WPO Noise Speed Y** | Animation speed on Y axis. | `1.0` |
