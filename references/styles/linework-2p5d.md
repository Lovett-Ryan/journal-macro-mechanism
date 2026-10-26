# Fine-line Diagram 2.5D

Style ID: `linework-2p5d`

## Visual intent

Build volume and hierarchy through fine contours, selective structural lines, and pale flat fills. Contours, structural turns, and clear boundaries dominate, producing a precise, light diagram rather than realistic scenery.

## Rendering rules

- **Form:** retain recognizable side faces, thickness, contacts, and occlusion. Simplified contours do not mean a flat flowchart.
- **Lines:** use a restrained weight hierarchy for principal outlines, internal structure, and secondary detail. Clean joins; no heavy black borders or dense wireframes.
- **Surfaces:** pale or unfilled faces with sparse texture. Use patterns selectively only when materials/layers need distinction; do not fill surfaces with grain, leaves, or reflections.
- **Continuous media/repetition:** simplified silhouettes, pale overlays, or a few informative boundaries. Group repeated objects rather than building realistic backgrounds from hundreds of details.
- **Light:** minor face-tone differences help orientation. Gradients, volumetric smoke, and shadows remain secondary; structural lines carry form.
- **Line roles:** distinguish contours, hidden structure, range boundaries, process arrows, and leaders. Auxiliary lines must not impersonate pathways.

## Adaptation for complex figures

- Beyond the main chain, branches, and feedback, retain only internal lines that help recognition. Reduce scene line density when explanations are numerous, not processes.
- Use pale planes/whitespace for labels. Process frames must differ from contours/hidden structure; keep outline and solid legend samples distinct.
- Avoid dense forests, granular media, mountain cracks, or equipment micro-parts turning the diagram into scenery or engineering wireframe.
- When switching, preserve geometry/information and translate material modeling into fine lines and pale faces without inventing structural edges.
- During removal, distinguish physical contours/structure from arrows/leaders/frames. Preserve the former and rebuild the latter in Visio; do not erase structural lines wholesale because they resemble overlays.

## Style prompt

```text
A precise, pale fine-line 2.5D scientific diagram with a coherent scene, meaningful side faces, thickness and readable interfaces. Define volume mainly through clean contours, selective structural lines, clear overlaps and light flat fills. Use a restrained hierarchy of line weights. Depict repeated objects as legible simplified groups and continuous media as a few informative shapes or boundaries rather than granular realistic rendering. Keep surface grain, gradients, highlights and shadows minimal. Retain every specified process and label while quieting decorative background detail. Distinguish physical outlines, hidden structures, range boundaries, process paths and annotation leaders. Keep text and the supplied legend encoding crisp and flat.
```

## Style-specific exclusions

```text
Avoid painterly scenery, photorealistic textures, densely repeated tiny objects, volumetric particle clouds, heavy cartoon outlines, sketchy strokes, decorative hatching, uniform wireframes, glossy materials and dramatic shading. Do not remove scientific depth or invent structural edges to fill space.
```

## Visible checks and correction

- Without texture, contours and pale faces still explain structure, thickness, and depth.
- Fine lines dominate rather than realistic materials/heavy shading. If it becomes scenery, simplify repeated objects/media and restore pale faces.
- Structural lines, pathways, and label frames have separate roles. Reduce secondary structure and reroute if tangled.
- Keep science and legend complete; do not sacrifice feedback for clean lines.
