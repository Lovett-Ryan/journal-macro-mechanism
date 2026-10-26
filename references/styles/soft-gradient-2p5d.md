# Soft Gradient 2.5D

Style ID: `soft-gradient-2p5d`

## Visual intent

Use clean geometry and broad continuous shading for volume, with smooth matte surfaces and sparse texture. Continuous modeling dominates rather than line density, material grain, or detailed terrain.

## Rendering rules

- **Form:** preserve key geometry, side faces, thickness, curvature, and structural edges. Gradients explain turns without rounding every object into a toy.
- **Light:** broad diffuse illumination, moderate transitions, consistent direction, faint contact shadows, and readable darker areas.
- **Surfaces:** distinguish materials mainly by intrinsic color, silhouette, and interfaces. Use little grain, scratching, or roughness texture.
- **Media:** when transparency is needed, show boundaries and visible interiors. Do not make solids transparent without scientific purpose or let overlapping colors alter semantic meaning.
- **Color:** shape gradients follow surface orientation; derive quantitative scales separately from evidence. Decorative shading is not a physical field.

## Adaptation for complex figures

- Model informative primary forms with gradients and quiet variations near text/paths. Use simplified related forms for small repeated objects.
- Keep labels, arrows, and legend flat and clear, without object lighting, gradients, or shadows. Semantic colors remain stable.
- For overlapping media, reduce scene color buildup or adjust whitespace to preserve endpoints, interfaces, and names. Do not cover them with large opaque cards.
- A style switch changes modeling only. Continuous shading must not alter structure, process direction, or relationship order.
- During removal, preserve continuous modeling, transparent media, and contact shadows with coherent repairs. Blur or vector flattening does not preserve materials. Place native Visio explanations over the retained raster treatment.

## Style prompt

```text
A softly shaded 2.5D scientific scene with clean geometry, smooth matte surfaces and broad, gentle continuous tonal transitions. Preserve all specified spatial relationships, side faces, thickness, structural edges and mechanisms. Use coherent diffuse lighting, restrained gradients and faint contact shadows; retain legible darker surfaces. Keep material texture sparse. Concentrate volume modeling on informative primary forms and quiet the areas behind annotations. Show transparent media only where required, with readable interfaces and interior geometry. Keep all text, pathway arrows and legend marks flat, crisp and stable in their semantic colors. Distinguish shape shading from evidence-based physical-field colors.
```

## Style-specific exclusions

```text
Avoid dense material texture, specular gloss, mirror reflections, harsh shadows, excessive ambient occlusion, uniformly rounded toy/clay shapes, decorative glow and gradients on text or arrows. Do not make every object transparent or invent physical-field gradients.
```

## Visible checks and correction

- Broad continuous transitions define primary forms with clear edges/thickness. Restore primary modeling if only flat fills remain.
- Surfaces are smooth rather than glossy plastic or rounded clay. Reduce reflections/contact shadows if heavy, without deleting geometry.
- Text/path regions remain quiet and transparent overlaps do not hide objects. Adjust scene gradients/opacity first if crowded.
- Do not remove all gradients to imitate minimal style or add natural texture merely to increase volume.
