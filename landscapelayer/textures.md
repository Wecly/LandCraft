# 🖼️ Textures

![](<../images/image28.jpg>)

Assign texture assets for the layer. Toggle which texture types are active based on your packed format.

---

### ♦ use Packed Normal

Switches Normal input to a packed format combining Normal + Roughness + Displacement in a single asset.

| Parameter | Description |
|-----------|-------------|
| **NRDp - use NDp** | Selects the packed layout: `NRDp` = Normal/Roughness/Displacement. `NDp` = Normal/Displacement without Roughness. |
| **use Roughness Texture** | Enables a separate Roughness texture instead of reading it from the packed Normal map. |
| **use Displacement Texture** | Enables a separate Displacement/Height texture. Required for POM and true displacement. |
| **use Packed Texture** | Enables a packed RGBA texture combining multiple material channels. |

---

![](<../images/image22.jpg>)

### Texture Slots

| Parameter | Description | Default |
|-----------|-------------|---------|
| **Albedo Texture** | Base color texture. | `T_pjwdt0_4K_B` |
| **Normal Texture** | Standard normal map. Used when Packed Normal is disabled. | `T_pjwdt0_4K_N` |
| **Displacement Texture** | Height/displacement map for POM and mesh displacement. | `T_Default_Mask` |
| **PackedNormal Texture** | Packed Normal + Roughness + Displacement texture. Active when `use Packed Normal` is enabled. | `T_PackedNormal` |
