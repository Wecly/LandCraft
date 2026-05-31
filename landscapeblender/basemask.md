# 🎭 Base Mask

![](<../images/image1.png>)

Defines the foundational mask that drives layer blending. Supports distance-based fading, slope masking, elevation masking, and Runtime Virtual Texture integration. The Base Mask determines where the top layer is visible over the bottom layer.

---

### 🚀 use Distance

Enables distance-based mask fading — the top layer fades out as the camera moves farther away.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Distance Offset** | Distance from camera at which the fade starts. | `10000.0` |
| **DistanceBlend Contrast** | Sharpness of the distance fade transition. | `8000.0` |

---

![](<../images/image4.jpg>)

### ♦ use RuntimeVirtualTexture

Uses a Runtime Virtual Texture as the source for the base mask data.

> Distance blend requires this checkbox when **Read from RVT** is enabled in Material Details Parameters.

---

### Combined Mask

| Parameter | Description |
|-----------|-------------|
| **🔴 Combined Mask** | Combines Slope and Elevation masks using logical AND — the top layer is only visible where both masks are active. |

---

![](<../images/image21.jpg>)

### 🔶 Slope Mask

Enables slope-angle-based masking — restricts the top layer to surfaces within a defined slope range.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Slope Facing Sun** | Limits the slope mask to surfaces facing toward the light direction. | — |
| **use Both Sides** | Applies the slope mask to both sun-facing and shadow-facing sides. | — |
| **use PixelNormals** | Uses pixel normals instead of vertex normals for slope calculation — more accurate on detailed surfaces. | — |
| **Slope Direction** | World-space direction defining the slope axis. | Blue (Z-up) |
| **Slope Amount** | Threshold controlling how steep the slope must be to trigger the mask. | `0.45` |
| **Slope Contrast** | Sharpness of the slope mask edge. | `1.0` |

---

![](<../images/image16.jpg>)

### 🔷 Elevation Mask

Enables elevation-based masking — restricts the top layer to a specific height range in world space.

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Elevation in Range** | Masks within a range above and below the Elevation Height instead of only above. | — |
| **Elevation Height** | World-space height at which the elevation mask activates. | `3000.0` |
| **Elevation Contrast** | Sharpness of the elevation mask edge. | `1.0` |
| **Elevation Range** | Width of the elevation range when `Elevation in Range` is active. | `1.0` |
