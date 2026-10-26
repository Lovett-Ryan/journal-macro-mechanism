# Minimal Color-block 2.5D

Style ID: `minimal-2p5d`

## Visual intent

Build spatial volume from concise silhouettes, smooth color blocks, and a few face-tone differences. Shape/plane relationships dominate. Keep the scene light and clear without reducing scientific information.

## Rendering rules

- **Form:** retain necessary side faces, thickness, relief, structure, and contact. Use representative shapes to reduce uninformative tiny parts without turning subjects into flat icons.
- **Shading:** a few stable face tones and faint contact shadows establish orientation; continuous gradients do not dominate.
- **Surfaces:** use sparse-texture matte fills. Distinguish materials through silhouette, intrinsic color, and clear interfaces. Retain scientifically meaningful layers and flow boundaries.
- **Repeated objects/media:** use representative groups to convey extent. Prefer clear contours and pale regions for continuous media rather than particles to prove realism. Preserve meaningful counts/distributions from the evidence.
- **Color:** harmonize scene colors, deriving semantic accents from the current mechanism rather than a fixed palette.

## Adaptation for complex figures

- Place the full chain, branches, feedback, and labels first, then reduce background repetition/decoration. Simplicity does not mean a handful of labels.
- Preserve whitespace within broad fills for text and paths. Keep object names, process outlines, and legends in their distinct [shared grammars](../style-guide.md), rather than turning them into large cards.
- Separate strata, media, and neighboring states with a few distinguishable planes. Do not merge process arrows and entity boundaries into one band.
- When switching styles, preserve scientific geometry/information and change surface rendering to discrete planes and concise silhouettes.
- During approved-figure removal, restore covered contours and face tones continuously, not with white patches. The raster retains scene color blocks; Visio rebuilds explanatory overlays only.

## Style prompt

```text
A clean color-block 2.5D scientific scene illustration. Preserve meaningful depth, recognizable side faces, thickness, interfaces and every specified mechanism. Define volume mainly with concise silhouettes and a small set of discrete, calm face tones. Use smooth matte fills, sparse surface texture and faint contact shadows. Group repeated background objects where their exact number is not meaningful; keep all scientifically significant objects distinct. Simplify decorative detail rather than processes, labels or feedbacks. Reserve quiet color fields for annotations and flat relationship graphics. Keep process paths distinct from physical boundaries, and preserve the supplied label and legend encoding.
```

## Style-specific exclusions

```text
Avoid photorealistic materials, dense granular surfaces, gradient-dominated modeling, glossy reflections, deep shadows, excessive tiny parts, heavy black outlines and toy-like forms. Do not flatten essential depth or remove mechanisms to achieve simplicity.
```

## Visible checks and correction

- Silhouette and a few tones explain forms, side faces, and thickness. Restore necessary volume if it looks like a flat flowchart.
- Unrelated surface detail is sparse, with complete structure and short labels. If content is missing, check mechanism coverage instead of adding decoration.
- If gradients or realistic textures dominate, return to discrete planes without changing scientific connections.
