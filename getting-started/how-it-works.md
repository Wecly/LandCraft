# How It Works

LandCraft is built around two core assets that work together:

* **ML\_LandscapeLayer** — a Material Layer defining how a single terrain surface looks: its textures, UVs, color, response, detail normals, deformation, variation, and grass maps.
* **MLB\_LandscapeBlender** — a Material Layer Blend that controls how two layers are composited together: which channels blend, how masking works, and how the blend transitions between layers.

You stack `ML_LandscapeLayer` instances in a landscape material and control each transition with an `MLB_LandscapeBlender`. Every parameter is exposed, grouped, and documented in this reference.

```
Layer  →  UV Logic  →  Textures  →  Color  →  Response  →  Detail  →  Deform  →  Variation  →  Grass Maps
```
