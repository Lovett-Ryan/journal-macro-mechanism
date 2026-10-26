# Relief Shading 2.5D

Style ID: `relief-2p5d`

## Visual intent

Use coherent slope shading, curvature, and structural turns to reveal the height and shape of existing surfaces. Macroscopic relief dominates; material grain/reflection stays secondary. The name does not require natural terrain in every scene.

## Rendering rules

- **Geometry:** preserve supported hierarchies of height, slope breaks, depressions, and rises. Flat surfaces stay flat; do not invent hills, cracks, or folds for style.
- **Light:** coherent soft directional light within a view; organize shading by slope/curvature. Emphasize primary relief, quiet secondary relief, and keep shaded faces readable.
- **Surfaces:** use geometry and shading rather than roughness/grain to explain relief. Avoid equal detail density everywhere.
- **Contours/cuts:** use auxiliary lines, contours, and cutaways for a scientific purpose. Layers come from structure, not shadows; quantitative contours require data.
- **Color:** maintain material classes across slope orientations. Define data scales separately; shaded faces are not different materials or lower-value zones.
- **Objects without relief:** treat planar parts, continuous media, and text according to their own forms, without universal terrain texture/shading.

## Adaptation for complex figures

- Concentrate relief shading on primary forms that affect paths, boundaries, or states. Lower contrast of minor relief near labels.
- Separate real grooves/channels from overlaid mechanism lines. Do not invent scientific routes by following shadows.
- Cutaways clearly show media boundaries; dark grooves do not substitute for interfaces. Text, arrows, and legend remain clear flat graphics.
- A style switch improves existing relief without changing meaningful slope, endpoints, quantitative geometry, or object classes.
- During removal, repair existing slope, curvature, and shading continuously, preserving channels, interfaces, and anchors. Retain raster relief while Visio restores flat explanations; do not replace surfaces with traced color patches.

## Style prompt

```text
A relief-shaded 2.5D scientific scene emphasizing the supplied macroscopic geometry. Reveal supported slopes, curvature, depressions and structural breaks through coherent, softly directional illumination. Establish a clear hierarchy of primary and secondary relief, with readable shaded faces and sparse material grain. Preserve genuinely planar surfaces and use appropriate simple treatment for objects without relief. Quiet minor shape variation behind labels and process paths. Keep physical channels and interfaces distinct from explanatory arrows. Apply contour lines and quantitative height or depth colors only when supported. Keep text and legend graphics flat and preserve scientific topology and semantic colors.
```

## Style-specific exclusions

```text
Avoid invented peaks, pits, folds, strata, excessive roughness, exaggerated relief, deep black crevices, uniformly dense detail, cinematic lighting and glossy materials. Do not add a mandatory landform, block base, contour system or elevation palette to every subject.
```

## Visible checks and correction

- Slope shading/curvature explain existing relief. If it resembles generic soft gradients, emphasize real primary relief without adding landforms.
- Planes remain planar and grain sparse. If it drifts toward Natural Texture, reduce grain/roughness while preserving geometric shading.
- Relief hierarchy, real interfaces, and process paths remain independently readable. Shadows do not hide text or imply unsupported values.
