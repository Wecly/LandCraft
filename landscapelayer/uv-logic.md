# 🗺️ UV Logic

![](<../images/image11.jpg>)

Controls UV projection, scaling, rotation, distance blending, tiling variation, and fake shadow. All UV behavior — from simple tiling to distance-based transitions — is managed here.

---

![](<../images/image23.jpg>)

### Base UV

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Slope Projection** | Projects UVs along the world-space slope direction — prevents texture stretching on steep terrain. | — |
| **Slope Axis Offset** | Offsets the slope axis reference direction. | — |
| **Scale** | Global UV tiling scale. | `10.0` |

---

### ♦ use Rotation

Enables UV rotation for the layer texture.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Rotation** | Rotation angle in degrees. | `0.0` |

---

![](<../images/image32.jpg>)

### ♦ use DistanceBlend

Enables distance-based UV blending — transitions to a different scale as the camera moves farther from the surface.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **DistantScale** | UV scale at far distance. | `10.0` |
| **use RuntimeVirtualTexture** | Uses RVT as the distant scale source. | — |
| **DistanceBlend Fade** | Fade range of the distance blend. | `8000.0` |
| **DistanceBlend Offset** | Start distance of the blend. | `10000.0` |

---

![](<../images/image25.jpg>)

### ♦ use Tiling Variation

Applies Voronoi-based tiling variation to break up visible texture repetition.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **use Tiling Variation Rotation** | Randomizes rotation per Voronoi cell. | — |
| **Voronoi Rotation** | Maximum rotation per cell. | `360.0` |
| **Voronoi Scale** | Scale of the Voronoi pattern. | `10.0` |
| **Voronoi Alpha Curve** | Blend curve at cell boundaries. | `10.0` |
| **Voronoi Offset Amount** | UV offset per cell. | `1.0` |

#### 🔷 use Distant Tiling Variation

Applies tiling variation at far distance — prevents repetition in the distant UV scale.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Distant Voronoi Offset Amount** | UV offset for distant Voronoi cells. | `10.0` |
| **Distant Voronoi Scale** | Scale of the distant Voronoi pattern. | `10.0` |

---

![](<../images/image27.jpg>)

### 🕯️ use Fake Shadow

Adds a height-based fake shadow — simulates contact shadow and depth without ray tracing.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Shadow Height** | Height threshold where the fake shadow starts. | `8.0` |
| **Shadow Steps** | Number of computation steps — higher is more accurate. | `16.0` |
| **Shadow Strength** | Intensity of the fake shadow effect. | `1.0` |
